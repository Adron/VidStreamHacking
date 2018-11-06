In bash, the shell reads one or more startup files. Here's the details about what's what and which is run when.

1. /etc/profile is executed automatically at login.
2. The file from the list of ~/.bash_profile, ~/.bash_login, or ~/.profile are then executed at login.
3. ~/.bashrc is executed by every non-login shell, but if sh is used to invoke bash it reads the $ENV for POSIX compatability.

For reference, the ~ symbol is used in place of the user directory. One way to check this out yourself is to change directory to ~ with a `cd ~` in the shell, then type `pwd` which will give the current directory. You'll find that it is something like `/Users/adron` where instead of my name it'd be your user name.

When invoking the shell, you can also skip the ~/.bashrc or otherwise change the way bash starts up with the following options.

* `bash --init-file theFileToUseInstead` or `--rcfile` instead of ~/.bashrc.
* `bash --norc` which is similar to invoking with `sh`, which will use $ENV.
* `bash --noprofile` will prevent /etc/profile or any other personal startup files. This will provide a pretty baseline bash shell for use.

Until next time, happy bash code thrashing!