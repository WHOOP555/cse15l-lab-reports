# CSE 15L Lab Report 1: Remote Access
---
1. ## Installing Visual Studio Code
    * The first step to logging into a course specific account on ieng6 is to install Visual Studio Code.
    * I already had Visual Studio Code installed on my device prior to this remote access lab, so I did not have to install it in this session.
    * If you do not have Visual Studio Code installed on your device, navigate [here](https://code.visualstudio.com/download) and download the version of Visual Studio Code that is compatible with your device and sufficient for your course. 
  ![image](https://user-images.githubusercontent.com/122576045/212810552-6c1e7d85-a977-454a-a5e0-62de1dd01e4e.png)
  ---
2. ## Remotely Connecting
   * First, navigate [here](https://sdacs.ucsd.edu/~icc/index.php) and discover what your course specific account and its username is. Then, reset your password, utilizing the aid of [this tutorial](https://docs.google.com/document/d/1hs7CyQeh-MdUfM9uv99i8tqfneos6Y8bDU0uhn1wqho/edit). Make sure to wait approximately 15 minutes after the password reset has finished to proceed, as the password change takes some time to register. Make sure you install [git](https://gitforwindows.org/) if you are using a windows device and set your default terminal to use git bash, as per [this tutorial](https://stackoverflow.com/a/50527994).
   * Next, open up a terminal in VSCode and type in the following command: `$ ssh cs15lwi23ddd@ieng6.ucsd.edu` with the "ddd" replaced by the letters at the end of your course specific account. If taking another course and/or during another quarter, make sure that you use your respective username instead of "cs15lwi23ddd". If a message prompts you to verify whether you do indeed want to continue to connect, affirm the request and then type your respective password.
   * You should now be connected and view some text like this in the terminal: <img width="467" alt="image" src="https://user-images.githubusercontent.com/122576045/212815184-b873658b-b752-4a7f-a711-329b96391483.png">
---
3. ## Trying Some Commands
   * When trying to list the files present in another student's account, utilize `ls <directory>` where "`<directory>`" is the respective student's directory, which can be in the format of "/home/linux/ieng6/cs15lwi23/cs15lwi23atr" where the last 3 letters are characteristic of the respective student's account. Here is an example of what attempting to access another student's account may look like:
  
  <img width="532" alt="image" src="https://user-images.githubusercontent.com/122576045/212816703-6f21aafa-f571-4f79-9d5b-8530c4b45536.png">
  
  * Some general commands to try are: `cd`, `ls`, `pwd`, `mkdir`, `cp`, `cat`. Some variations can be added to these general commands, such as `ls -lat`, which may result in something like this: 
  
  <img width="489" alt="image" src="https://user-images.githubusercontent.com/122576045/212817341-170116ef-0939-4546-ade7-acaeabd294e4.png">
  * Finally, to exit remote server, simply run the `exit` command, which may produce a result like this: 
   
   <img width="246" alt="image" src="https://user-images.githubusercontent.com/122576045/212817736-7f15171e-688f-4bbb-851c-7e01db1cd713.png">
