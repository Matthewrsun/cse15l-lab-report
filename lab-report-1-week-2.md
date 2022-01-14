# Week 2 Lab Report

## Installing VSCode

To install VSCode, visit the Visual Studio Code website at [this link](https://code.visualstudio.com/). Pick the version for your operating system, and once you finish downloading VSCode, run the program. A window should appear like the one below:

![vsc pic](Lab1-1.png)

## Remotely Connecting

The next step is to be able to connect to a remote server. For this, we're going to use a program called OpenSSH, which can be downloaded here: [OpenSSH Install Instructions](https://docs.microsoft.com/en-us/windows-server/administration/openssh/openssh_install_firstuse). After this, you can login to the remote ieng6 server using your unique student account, which can be found here: [UCSD Account Finder](https://sdacs.ucsd.edu/~icc/index.php). You can also find and change your account's password there too.

![account finder](Lab1-2b.png)
Now, you are able to login to a remote server using the VSCode terminal. Open up a terminal and run this code:

`$ ssh cs15lwi22ahf@ieng6.ucsd.edu`

Don't forget to replace the letters after "wi22" with your personal account! Enter your password and you should be in!

![ssh login](Lab1-2.png)

## Trying Some Commands

Once you're in, you can try using some commands in the server. Some such commands include:

```
cd ~
cd
ls
ls -lat
ls -a
```

Here is an example, where I ran the command `ls -a`.

![ls -a](Lab1-3.png)

## Moving Files with `scp`

A command we are going to use now is `scp`, which copies a file from the client (the device you're using) onto the server. This command is run from the client. In my example, I used a file called WhereAmI.java. The command I used was this:

`scp WhereAmI.java cs15lwi22ahf@ieng6.ucsd.edu`

![scp1](Lab1-4.png)

A prompt will pop up asking for your password, similar to when you were logging in, and after you enter your password, you should be able to see that your file has been copied over. Now, you will be able to find the file in the server directory.

![scp2](Lab1-4b.png)