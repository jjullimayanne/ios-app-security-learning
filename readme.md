
#### IOS Basic Tests


#### You will need: if you have a jailbroken device: 

- embedded.mobileprovision
- What is a provision? 

Provisioning profile act as a link between the device and the developer account. 

Then: 
~~~
npm install -g applesign 
~~~
To list your applesign 
~~~
 applesign -L 
~~~

~~~
 applesign -i <YOUR APPLESIGN> <APPNAME> -m <embedded.mobileprovision>
~~~


#### You will need: if you have a non-jailbroken device: 

- Fist of all download and install `objection` in this link:

[Objection page](https://github.com/sensepost/objection)

 What does Objection mades? 
Objection is a runtime mobile exploration that help you assess the security posture of mobile applications. 

- Use this code to sign with your `applesign`:
~~~
objection patchipa --source SecureStorev2.ipa --codesign-signature <YOURSIGN> -P embedded.mobileprovision
~~~

This will generate a new file that will be signed 

- Zip your file generate through the previos command:
~~~
 cp YOURGENERATEAPP frinda.zip  
~~~

- Unzip your file again because you need the payload folder

- You also will need run frida 

~~~
unzip frida.zip
~~~

-Now you need install `ios-deploy`

~~~
npm install ios-deploy
~~~

- Inside the payload folder you will need run a command to deploy your app 

~~~
 ios-deploy --bundle SecureStorev1.app -d -W
~~~

- Now runs Frida command to acess de app:

~~~
 frida -U -n "AppName"
~~~

Frida is a instrumentation for reverse-enginners, security and etc. 
[Frida](https://github.com/frida/frida)




[Database](https://drive.google.com/drive/folders/14SGvrAdsoZJiWz93E3Jm-WBsy8KouOiP?usp=sharing)

username | password

+----+-----------------------+-

securestore | securestore

attacker       | attacker










