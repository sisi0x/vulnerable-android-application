 That very important to focus if the application show the username or password or credit card in logs as clean text or not

And lieek http reqoust 
and root dection bypass 

##### The firs step we need the package name and `id` and use adb logcat 

1- To know all packages used the Command : adb shell pm list packages

![Screenshot 2024-04-26 064028](https://github.com/sisi0x/vulnerable-android-application/assets/100969542/40f3acec-2c58-4587-9b9c-d9a02cb32647)



2- Then we need Know what is pidof we need `Package Name` 
Command : adb shell pidof -s  "Package Name"


 ![Screenshot 2024-04-26 064404](https://github.com/sisi0x/vulnerable-android-application/assets/100969542/b2e76da8-fb0e-42e6-877b-a5a5a8ce16d1)


3- Then listen
Command:  adb logcat --pid=4813

![Pasted image 20240426065150](https://github.com/sisi0x/vulnerable-android-application/assets/100969542/5f9cfd0f-f141-45f6-84c5-ca0f8487febe)



Mitgition :
Don't using function Log with sensitive data
