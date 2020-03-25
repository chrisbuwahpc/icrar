# small

This project is for using vagrant and virtualbox to manage the environment for 
the Software Carpentry Training course.

##  setup 

In the same directory where the small directory is going to be installed 
create a directory named *scripts*

```bash 
tmep >ls
tmep >mkdir scripts
tmep >git clone https://github.com/chrisbpawsey/small.git
Cloning into 'small'...
remote: Enumerating objects: 14, done.
remote: Counting objects: 100% (14/14), done.
remote: Compressing objects: 100% (9/9), done.
remote: Total 14 (delta 3), reused 14 (delta 3), pack-reused 0
Unpacking objects: 100% (14/14), done.
tmep >ls
scripts	small
```

Now you are ready to start vagrant!

```bash
cd small
```

You should find a file *Vagrantfile* that is used to start and 
provision your instance!

The command to use is 
```bash
vagrant up
```

To login to your instance the command is:
```bash
vagrant ssh
```


-----------------------

## Basic Vagrant Commands
virtual >vagrant --help
Usage: vagrant [options] <command> [<args>]

    -v, --version                    Print the version and exit.
    -h, --help                       Print this help.

### Selected commands:
```bash
     destroy         stops and deletes all traces of the vagrant machine
     halt            stops the vagrant machine
     help            shows the help for a subcommand
     init            initializes a new Vagrant environment by creating a Vagrantfile
     ssh             connects to machine via SSH
     up              starts and provisions the vagrant environment
     version         prints current and latest Vagrant version
```
For help on any individual command run `vagrant COMMAND -h`

Additional subcommands are available, but are either more advanced
or not commonly used. To see all subcommands, run the command
`vagrant list-commands`.


