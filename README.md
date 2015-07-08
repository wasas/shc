# Shell Script Compiler

	A generic shell script compiler. Shc takes a script, which is
	specified on the command line and produces C source code. The
	generated source code is then compiled and linked to produce a
	stripped binary executable. Use with care.

Install:
--------
	cd to directory "main": cd main
	do a "make"
	and then "sudo make install"

	or simply run the "install" script/file provided, in terminal

Usage:
------
```
shc [options]
shc -f script.sh -o binary
```

N.B: The binary still requires the relevant shell to be available in the system to be run.


Testing:
--------
	cd to test "directory": cd test
	Try: shc -f test.bash -o test

	output binary file will be test. If no output file is specified
	by the -o option, then it will create an executable with .x extension
	by default


Known bugs:
-----------

	The one (and I hope the only) limitation using shc is the
	_SC_ARG_MAX system configuration parameter.

	It limits the maximum length of the arguments to the exec function,
	limiting the maximum length of the runnable script of shc.

	!! - CHECK YOUR RESULTS CAREFULLY BEFORE USING - !!
<h2><a href="http://neurobin.github.io/shc">WebPage</a></h2>
