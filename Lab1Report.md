#***Step 1: Installing VScode***1
---
I didn't have to install VScode, as I already had it installed from when I took CSE 11. 
After installing Vscode however, you should be able to open and launch a window similar to the image below.
![Image](VScodeWindow.png)

#***Step 2: Remotely Connecting***1
---
In order to remotely connect to an online server, you must first install Git for Windows. 
After the installation is complete, open VScode and open the search bar by holding ***ctrl*** + ***shift*** + ***p***.
Type ***Select Default Profile***.
Select ***Git Bash***.
Next, open a terminal by clicking on the terminal tab at the top of your screen and select ***New Terminal***.
Type ***ssh cs15lwi23zz@ieng6.ucsd.edu***, where zz are the letters of your course account.
In order to find the letters of course account, go to https://sdacs.ucsd.edu/~icc/index.php and follow the instructions there to lookup your account and reset your password.
Type yes and enter the password that you created to login into your account. 
You should now see the image below.
![Image](RemoteControl.png)

#***Step 3: Trying Some Commands***1
---
I tested some commands after on the remote connected terminal such as 
*cd 
*ls 
*pwd 
*mkdir
*cp 
*cd~
*ls -lat
*ls -a 
*ls <directory>, where <directory> is /home/linux/ieng6/cs15lwi23abc, where abc is one of the other group members'username
*cp /home/linux/ieng6/cs15lwi23/public/hello.txt ~/ 
*cat /home/linux/ieng6/cs15lwi23/public/hello.txt
It should look something like the image below.
![Image](Command.png)
