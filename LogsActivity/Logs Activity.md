 That very important to focus if the application show the username or password or credit card in logs as clean text or not

And lieek http reqoust 
and root dection bypass 

##### The firs step we need the package name and `id` and use adb logcat 

1- To know all packages used the Command : adb shell pm list packages

![[Screenshot 2024-04-26 064028.png]]

2- Then we need Know what is pidof we need `Package Name` 
Command : adb shell pidof -s  "Package Name"
 
![[Screenshot 2024-04-26 064404.png]]

3- Then listen
Command:  adb logcat --pid=4813

![[Pasted image 20240426065150.png]]

Mitgition :
Don't using function Log with senet