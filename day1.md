# Linux Basics Course
 
## Why learn Linux? 
- 96% top million web servers runs on Linux
- 86% smartphones powered by Linux
- Cloud and DevOps tools are used in Linux
- Docker 2013-Linux -- Docker, anisible and kubernetes Was only for linux untill 2016 - Windows


## Introduction to Shell: 
Shell - Linux command-line interface that allows text based interaction between user and OS

Home Dir- system created directory, contains home dir for all users
- home dir is unique for each users
- home dir is represented by tilde symbol [~]
- allows users to store personal data

## Commands and Arguments
command- executes a program to achieve a specific task
Argument- input to the command
Option/switch/flag- modify behavior of a command 
 
Commands Types:
- Internal or Built-in Commands - part of shell or built in command. 
- External Commands - binary programs or scripts. Can be pre-installed or installed by user
- Use <type> command to check the type of command
 
## Basic Linux commands

echo -- print in the terminal 

uptime --how long the system has been running for?

type < command > -- shows the type of command

pwd -- present working directory 

ls -- list contents
ls -l -- long list, displays accessed list, owners, permissions and last accessed.
ls -a -- displays all the files and dir including hidden ones[.]
ls -lt -- order that the file is last modified, newest to oldest
ls -ltr -- oldest to newest 

mkdir -- make directory 
mkdir apple/mango -- creates dir mango inside apple dir
mkdir -p apple/mango -- creates parent dir. creates both apple and mango

cd change directory 
pushd -- remembers the current working dir before changing to the dir specified
popd -- return back to the original dir 

- Absolute Path: Location of a file or a dir starting from a root dir -- /home/tobden/file
- Relative Path: Path in relation with the present working dir file

mv -- move files and dir -- rename dir
mv /dir/you/want/to/move /destination/dir
mv /oldname /newname

cp -- copy files and dir 
cp /source/file /destination/file
cp -r /source/dir /destination/dir -- recursive

rm -- to remove files

cat -- concatante -- to read files
cat > -- to add datas to a file [ctrl + d ] to save and exit

touch -- to create new empty file

- Pagers: more and less commands. To read or view the contents of a file. 

more -- similar to cat, read datas in scrollable manner but loads all the content at once. [space]-scroll page [enter]-scroll line [b]-scroll back [/]-search text [q]-exit
less -- read the files and navigate through the file [up]-scroll up [down]-scroll down [/]-search [q]-exit 

## Getting Help in Command Line
whatis < command > -- 1 line description of what the command does
man < command > -- detail info of the command with examples, use cases and info about options
< command > --help -- provides with options and use cases of the command
apropos < command/keyword > -- search through the man page names that matches the keyword

## Shell Types
- Faclitates the communication between the user and the OS 

echo $SHELL -- to check the shell being used
chsh -- to change the default shell

- Bourne Shell
- C Shell
- Korn Shell (ksh)
- Z Shell (zsh)
- Bourne again Shell (bash)

Bash Shell Features 
- Bash Auto-Completion
- Custom alias 
alias < custom command >=< existing command >
history -- to check the history of command used

## Bash Environment Variables
Enviroment variables - stores info about the user's login session used by the shell when executing commands

env -- to check all the env variables used
export OFFICE=selise -- to set an env variable
OFFICE=selise -- will only set variables within the shell -- to make variables presistent pver subsequent login or reboots add to  [.profile] or [.pam_enviroment] file

- Path Variable - when user issues an external command into the shell, shell uses a path variable to search for these external commands.

echo $PATH -- to see the dir defined in the path variable
which < command > -- to check if the location of a command can be identified 
export PATH=$PATH:/opt/pbs/bin

## Bash Prompt 
- provides meaningful info about the logged in user, name of the system and the location on the system. Can be customized.

[~]$ -- bash prompt
~ -- present working dir 
$ -- user 

PS1 -- special shell env variable that controlls bash prompt 
PS1="< name >" -- Customizing Bash Prompt by updating the PS1 variable

\d -- date week/month/date format
\h -- hostname
\H -- complete hostname
\n -- newline
\r -- carriage return 
\s -- shell name
\t -- current time in 24hr HH:MM:SS 
\T -- current time in 12hr HH:MM:SS
\@ -- current time in 12hr am:pm
\A -- current time in 24hr HH:MM 
\u -- current logged in username
\w -- basename of the current working dir with $HOME abbreviated with a tilde
\e[< colorcode textcolor >:< colorcode background color >m\] -- set the color of the bash prompt

PS1="\e[36m\]\u@\h:\w " -- example

Package Management 
- .DEB - Ubuntu, Debian, Linux Mint
- .RPM - RHEL, Centos, Fedora
Softwate Package - 

# Table of Contents

1. [This is my content](https://mail.google.com/mail/u/0/#inbox)
