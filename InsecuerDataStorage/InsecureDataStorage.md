The Source code

![Pasted image 20240426120319](https://github.com/sisi0x/vulnerable-android-application/assets/100969542/7825a627-7d2f-4b19-b754-8420f61166af)

Let's start to  analyzing the code is very simple, we have to enter the first username and the second password and take the username and password to store in Default Shared Preferences as clean text , Here is an issue

### To see the data
\Go in `data\data` and select the `package name` 
Command : cat jakhar.aseem.diva_preferences.xml


![Screenshot 2024-04-26 115908](https://github.com/sisi0x/vulnerable-android-application/assets/100969542/21c19acb-3cdf-4b87-ad9c-6da612790fdc)

we don't recommend stored any sensitive data like username or password or credit card as clean text in Shared Preferences and we not recommend using Shared Preferences


Mitigation : recommendation using data stored or  KeyChain 
why using data stored?
beause wan used data stored you need key and value, rembambr using Encrypt like AES and the backmod is cbc

https://developer.android.com/reference/android/security/KeyChain.html
