#Introduction
Project is mini bash implementation called Free shell (fsh). It has support of some built-in functions, can also execute programs using full path or using $PATH envirovent variable, and joint multiple commands using ; && || operands.

###External Libs
Free shell uses third party library 'read-line'.

read-line library installation instructions for Ubuntu.
```bash
sudo apt-get update
sudo apt-get install libreadline6 libreadline6-dev
```

#Usage
Program execution is simple.
```bash
sudo ./fsh
```

##Feature
```
Free shell (fsh) has built-in functions: ?, cd, exit, kill, pwd, ulimit, nice, echo, type, export.
It can also execute executable files and to find and execute executable programs in the folders of the $PATH.
Free shell can join commands in several ways.
; = Is same as new line.
&& = Runs the next command only if the latter one exited without error.
|| = Runs the next command only if the latter one exited without error.
< = Redirects STDIN
> = Redirects STDOUT
>> = Redirects STDOUT into the file. 
 ფუნქციებს, ასევე შეუძლია კონკრეტული გაშვებადი ფაილების გაშვება, ან/და ფაილების მოძებნა PATH გარემოს ცვლადის მიერ მითიტებულ

```

#Project Structure

###Tree
```
.
├── built_in_functions
│   ├── about.c
│   ├── about.h
│   ├── cd.c
│   ├── cd.h
│   ├── echo.c
│   ├── echo.h
│   ├── execute.c
│   ├── execute.h
│   ├── execute_path.c
│   ├── execute_path.h
│   ├── exit.c
│   ├── exit.h
│   ├── export.c
│   ├── export.h
│   ├── kill.c
│   ├── kill.h
│   ├── nice.c
│   ├── nice.h
│   ├── pwd.c
│   ├── pwd.h
│   ├── type.c
│   ├── type.h
│   ├── ulimit.c
│   ├── ulimit.h
│   ├── utility.c
│   └── utility.h
├── controller.c
├── controller.h
├── main.c
├── Makefile
├── parser.c
├── parser.h
└── README.md
```

###makefile
Project is built using [make](http://www.gnu.org/software/make/manual/make.html),
file contains instructions for [make](http://www.gnu.org/software/make/manual/make.html)
to build project.

###README.md
readme of the project.
