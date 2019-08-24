#  Lab exercise 1 objectives
1. Set up Tuffix environment
2. Modify and compile C++ programs
3. Run program and test input/output

# Additional Reading
Chapter 1 of the course textbook.

# Instructions
Answer the programming problems sequentially (i.e., answer prob01 before prob02). If you have questions let your instructor or the lab assistant know. You can also consult your classmates.

# Lab exercise guide
Here's a link to the [Lab exercise guide](https://drive.google.com/open?id=1MCaTFhxM1wIeC-Iwr1FC4Fw1mVVVRXh7) in case you need to review the lab exercise objectives, grading scheme, or evaluation process.

# Code evaluation
Open the terminal and navigate to the folder that contains this exercise. Assuming you have pulled the code inside of `/home/student/labex01-tuffy` and you are currently in `/home/student` you can issue the following commands

```
cd labex01-tuffy
```

You also need to navigate into the problem you want to answer. To access the files needed to answer problem 1, for example, you need to issue the following command.

```
cd prob01
```

When you want to answer another problem, you need to go back up to the parent folder and navigate into the next problem. Assuming you are currently in `prob01`, you can issue the following commands to go to the parent folder then go into another problem you want to answer; `prob02` for example.

```
cd ..
cd prob02
```

Use the `clang++` command to compile your code and the `./` command to run it. The sample code below shows how you would compile code saved in `main.cpp` into the executable file `main`. Make sure you use the correct filenames required in this problem.  Take note that if you make any changes to your code, you will need to compile it first before you see changes when running it.

```
clang++ -std=c++17 *.cpp -o main
./main
```

# Submission
1. To upload your code into the GitHub repository, the first step is to add your code to what is called the staging area using git's `add` command. The parameter after `add` is the name of the file you want to add. There are cases when you have multiple changed files, so you can just type . (period) to add all modified files.

    ```
    git add .
    ```

1. Once everything is in the staging area, we use the `commit` command to tell git that we have added everything we need into the staging area. This command can be issued with a message informing users of the changes made.

    ```
    git commit -m "short description of code changes being uploaded"
    ```

1. In case it asks you  to configure global variables for an email and name, just copy the commands it provides then replace the dummy text with your email and GitHub username.

    ```
    git config --global user.email "tuffy@csu.fullerton.edu"
    git config --global user.name "Tuffy Titan"
    ```

    When you're done, make sure you type the `git commit` command again.

1. And finally, you can upload all changes to the GitHub repository using git's `push` command. Provide your GitHub username and password when you are prompted for these.

    ```
    git push
    ```

1. When you finish the exercise, go back to Titanium and click on the `Add submission` button in the lab exercise page. Provide a short message *that includes your GitHub username* in the text area such as "user tuffy - finished lab exercise" and click on `Save changes`. Finally, click on `Submit assignment` to inform your instructor that you are done.
