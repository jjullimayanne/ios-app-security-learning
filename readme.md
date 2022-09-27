
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
 cp YOURGENERATEAPP YOURGENERATEAPP.zip  
~~~

- You also will need run frida 








