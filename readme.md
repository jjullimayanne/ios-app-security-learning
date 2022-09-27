
#### IOS Basic Tests


#### You will need: if you have a non-jailbroken device: 

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







