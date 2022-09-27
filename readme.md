
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

Fist of all download and install `objection` in this link:

[0BJECTION](https://github.com/sensepost/objection)

- What does Objection mades? 
Objection is a runtime mobile exploration that help you assess the security posture of mobile applications. 






