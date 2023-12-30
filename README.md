# cs1b_hw02_template
## Using functions and the `make` utility

This is basically the same program as assignment **hw01** except the calculation is coded on a separate file `hw01f.cpp` and compilation is managed by the utility `make`, as discussed in class.  Make sure that the configuration of the `Makefile` minimizes recompilation upon individual changes, also as discussed in class.  During development, use `git` with at least two commits and `git push` the code to your github.com repository.

Write a program that takes a variable amount of scores (less than 50) and outputs the average of the scores.  Use a array of type `double` to store each score. Include a header file with your personal information, pre-processor directives, etc. Notice that the function prototype (`calculateAverate()`) is given to you in the header file `hw02.h`.  Do not change the function signature or return type as the automated unit test will fail if so.

Perform the following commands to generate the `tar` package:

`cs1stud@cs1vbox:~/cs1b/hw02$ script hw02.scr` <br/>
`cs1stud@cs1vbox:~/cs1b/hw02$ ls -l` <br/>
`cs1stud@cs1vbox:~/cs1b/hw02$ make` <br/>
`cs1stud@cs1vbox:~/cs1b/hw02$ ./hw02` <br/>
`Enter score: 96` <br/>
`Enter score: 81` <br/>
`Enter score: Ctl-D` <br/>
`The average is 88.5` <br/>
`cs1stud@cs1vbox:~/cs1b/hw02$ git log > hw02git.log` <br/>
`cs1stud@cs1vbox:~/cs1b/hw02$ Ctl-D` <br/>
`Script done, file is hw02.scr` <br/>
`cs1stud@cs1vbox:~/cs1b/hw02$ tar cf hw02.tar hw02.h hw02.cpp hw02.scr hw02git.log` <br/>


Note: Do NOT include compiled binaries (ie, `hw02`, `hw02f.o`) in the `tar` package file.
