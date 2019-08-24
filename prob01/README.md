# Lab exercise 1 objectives
1. Navigate and explore Tuffix, a Linux environment.
2. Update C++ code on the Atom editor.
3. Navigate the Linux file system using a command line interface (CLI).
4. Compile C++ code.
5. Run compiled code (executable files).
6. Use git to add and commit code to the local staging area as well as push code to a Github repository.

# Instructional videos
Here are some instructional videos that you can view to know more about Tuffix and the command line.
1. Running Tuffix using Virtual Box (https://youtu.be/otB9FPC86a8?t=1m54s)
2. Intro to Tuffix (https://youtu.be/c0ZrWmarSwI)
3. Intro to the Linux command line (https://youtu.be/bQm8TUTDK7E)
4. Intro to Atom and clang++ compilation (https://youtu.be/TYlg3Ka8Mos) (Replace all the g++ commands with clang++)

# Instructions
Follow the steps listed below to complete this lab exercise.
1.  Make sure that the shared clipboard of VirtualBox is set to *Bidirectional* to allow you to easily copy and paste text between your host operating system and your virtual machine.
 ![Setting shared clipboard to bidirectional](https://www.dropbox.com/s/szet7dsy2118mmo/Shared%20clipboard.png?raw=1)
1. Open the Terminal in Tuffix through the Whisker menu.
1. Make a copy of this Github repository on your computer using the `git` and `clone` commands that you will input to the terminal. The commands take a URL as a parameter to specify where it can get a copy of the repository. You can find the URL by clicking on the green *Clone or download* button at the top right part of this page.

    Copy the URL and replace the dummy text shown below. When you hit <kbd>Enter</kbd> it will ask you to provide your Github username and password. Provide the information to start the cloning process. Once done, you will have a copy of the repository on your computer.

    ```
    git clone place_URL_here
    ```
    You should now have a copy of the files on your machine.
1. Navigate into your labex1 folder using the command line. Take note that this will vary per user because the folder name is based on your Github username. The example below assumes the user's username is Tuffy. Replace it with your own folder name. Take note that you can type the first few letters of the folder name and press <kbd>Tab</kbd> so that it auto completes the folder name for you.

    ```
    cd labex01-your_github_username_here
    ```
1. Navigate to the prob01 folder using the following command.
    ```
    cd prob01
    ```

1. Compile the prob01 code using the command below. The `-std` option tells the compiler that it will use C++ version 17 standards and the `-o main` option tells the compiler to place the executable code into a file called `main`.

    ```
    clang++ -std=c++17 main.cpp -o main
    ```
1. Run the program using the command below

    ```
    ./main
    ```
1. Use the Atom editor to open the file called *main.cpp* inside of your lab exercise 1 prob01 folder.
1. Edit the "hello world" message so that your program will write something different to the console
1. Compile and run your program again.
1. When everything runs correctly, copy your code into the Github repository. The first step is to add *main.cpp* to what is called the staging area using git's `add` command. The parameter after `add` is the name of the file you want to add. Optionally, you can type . (period) if you want to add all modified files.

    ```
    git add main.cpp
    ```
1. Once everything is in the staging area, use the `commit` command to tell git that we have added everything we need into the staging area.

    ```
    git commit -m "changed hello world message"
    ```
1. In case it asks you to configure global variables for an email and name, just copy the commands it provides then replace the dummy text with your email and Github username.

    ```
    git config --global user.email "tuffy@csu.fullerton.edu"
    git config --global user.name "Tuffy Titan"
    ```
    When you're done, make sure you type the `git commit` command again.
1. Finally, push all changes to the Github repository using git's `push` command. Provide your Github username and password when you are prompted for these.

    ```
    git push
    ```
1. Congratulations, you have now completed your C++ project on Github! Refresh the Web page and you should see the changes to the *main.cpp* file that you pushed from your command line.
