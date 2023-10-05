# Hi this is Charlie Shang
## Lab 1 Report
### 1. cd with no argument
![Image](cd_no_arg.png)<br />
* working directory: `/home`
* There are no output, because `cd` means change directory and will not give output. Also, the directory does not change because there is no argument for `cd`, which is like `cd .`, which means does not change directory or change the directory to the current directory.
* The output is not an error. `cd` nothing just means that does not change the directory.

### 2. cd with directory argument
![Image](cd_arg_dir.png)<br />
* working directory: `/home`
* As above mentions, `cd` does not generate output. However, since here we have a directory as an argument, our directory actually changes. The directory changes from /home to `/home/lecture1`. If the argument is something other than lecture1, the directory will not change because under `/home`, there is only one directory which is `/lecture1`.
* The output is not an error. It successfully changes the directory from `/home` to `/home/lecture1`.

### 3. cd with file argument
![Image](cd_arg_file.png)<br />
* working directory: `/home/lecture1`
* There is an output which shows that file `en-us.txt` is not a directory.
* The output is an error. It makes sense because `cd` means change directory, and the argument of cd has to be a existing directory. Otherwise, it will cast error. In this case, `en-us.txt` is a file instead of a directory, which is the reason why error occurs.

### 4. ls with no argument
![Image](ls_no_arg.png)<br />
* working directory: `/home`
* The command `ls` without argument means list the directories or files under the current directory. Therefore, the working directory is `/home`, so the output is what in the `/home` directory, which is `/lecture1` directory. 
* The output is not an error. `ls` without argument is printing out what is in the working directory.

### 5. ls with directory argument
![Image](ls_arg_dir.png)
* working directory: `/home`
* The command `ls` with argument means list the name of directories or files under the directory given as argument. As we are in `/home` directory, and the argument we pass is `/lecture1`, it will show the name of all directories and files under `/home/lecture1`, which is exactly what the output is.
* The output is not an error. It correctly outputs the name of directories and files under the argument we pass in.

### 6. ls with file argument
![Image](ls_arg_file.png)
* working directory: `/home`
* I actually have never tried to pass a file as the argument of `ls` before. According to the output shown on the picture and several tests I tried on my own terminal, I found that `ls` with file passed as argument prints the directory of the file starting from the working directory. According to the picture above, we are at `/home` directory, and the argument passed in is `en-us.txt` file under `/home/lecture1/message`. The output is `lecture1/message/en-us.txt`, which is the directory of the file starting from the working directory.
* Although I am not sure, I do not think this is an error. I think `ls` used with a file should print its directory starting from the working directory.

### 7. cat with no argument
![Image](cat_no_arg.png)
* working directory: `/home`
* There is no output. However, the terminal kept running until I click on `ctrl+C` to stop it. Therefore, there is no output if I use `cat` with no argument. This will keep the terminal running.
* It is an error, because `cat` with no argument keeps terminal running and does not stop. `cat` reads data from the file passed as an argument and prints the content. However, since we do not pass in any argument, `cat` cannot read anything and thus error occurs.

### 8. cat with directory argument
![Image](cat_arg_dir.png)
* working directory: `/home`
* The output is a message saying that `/lecture1` is a directory. This message occurs because `cat` command is to read data from the file passed as an argument and prints the content. The argument has to be a file, not a directory. Therefore, the terminal is warning us that the argument we pass in is not what `cat` wants.
* It is an error, because `cat` should get a file as an argument to correctly print the content of the file as output. Since we pass in a directory as argument, the error occurs.

13. cat with file argument
![Image](cat_arg_file.png)
* working directory: `/home`
* The output is `Hello World!`, which is the content in the file `en-us.txt`. As mentioned above, `cat` reads data from the file passed as an argument and prints the content. Since we successfully pass a file as the argument, the terminal correctly prints out the content in that file.
* It is not an error, because we pass in argument as `cat` wants, which is a file. Therefore, the terminal successfully prints the correct output.
