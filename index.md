# Hi this is Charlie Shang
## Lab 1 Report
1. cd with no argument
![Image](cd_no_arg.png)
working dir: /home

There are no output, because cd means change directory and will not give output. Also, the directory does not change because there is no argument for cd, which is like cd ., which means does not change directory or change the directory to the current directory.

The output is not an error. cd nothing just means that does not change the directory.

3. cd with directory argument
![Image](cd_arg_dir.png)
working dir: /home

As above mentions, cd does not generate output. However, since here we have a directory as an argument, our directory actually changes. The directory changes from /home to /home/lecture1. If the argument is something other than lecture1, the directory will not change because under /home, there is only one directory which is lecture1.

The output is not an error. It successfully changes the directory from /home to /home/lecture1.

5. cd with file argument
![Image](cd_arg_file.png)
working dir: /home/lecture1

There is an output which shows that file en-us.txt is not a directory.

The output is an error. It makes sense because cd means change directory, and the argument of cd has to be a existing directory. Otherwise, it will cast error. In this case, en-us.txt is a file instead of a directory, which is the reason why error occurs.

7. ls with no argument
![Image](ls_no_arg.png)
working dir: /home
8. ls with directory argument
![Image](ls_arg_dir.png)
working dir: /home
9. ls with file argument
![Image](ls_arg_file.png)
working dir: /home
10. cat with no argument
![Image](cat_no_arg.png)
working dir: /home
11. cat with directory argument
![Image](cat_arg_dir.png)
working dir: /home
12. cat with file argument
![Image](cat_arg_file.png)
working dir: /home
