Mean Period 6
=======
####Explain the concept of Hybrid Mobile App Development
The concept about hybrid apps are that you are able to create a mobile application via webtechnologies and then use Cordova/PhoneGap as a layer to intepret the web code to native code. Thereby making app creation for multiple platforms easy.
Explain the Pros & Cons of using Hybrid Mobile App Development compared to Native App Development
Hybrid apps are very easy to create and only demands a programmer with knowledge to webtechnologies. You only need one code base to compile for android, ios etc.
The disadvantage is speed and some native specific functions to be unavailable.

####Explain about the "building blocks" involved in an ionic Hybrid Application
The building blocks of a Hybrid app has three key blocks. 

- The codebase: made with webtechnologies
- Compiler: PhoneGap/Ionic
- Runtime: Native platform

![alt tag](http://india.nextremer.com/img/service/Hybrid-app-devlopment.PNG)

####Explain and demonstrate ways to debug Hybrid Mobile Applications Running on a real device.
- Enable USB debugging on your device: 
- Open Chrome on your desktop (development) machine and navigate to: chrome://inspect
- Select Discover USB Devices.
- Select your device.
- To use your device to debug a web application that’s running on your development machine:
- Click Port forwarding….
- Set the device port and the localhost port.
- Select Enable port forwarding. 

####Explain when and why CORS is a problem for Hybrid Mobile Applications
Usually you will have an application that uses a backend an sends and recieves data from somewhere else - this can cause a problem as your backend would not allow request from unspecified addresses. 
To solve this you can either make a Access-Control-Allow-Origin * to allow request from all locations - or specify the request to go through a proxy and then allowing the proxy to talk to the backend.
If you dont want to spend time creating the backend you can use Firebase which also solves the CORS problem.

####Explain how and why it is possible for a Hybrid Application to access native phone devices like location, calendar etc.
Using a native wrapper like Cordova grants you the possibility to compile to native application language. Also there are plugins like GeoLocation and Ionic Keyboard which is created to communicate with native mobile functions. This is a good way to create almost similar to native applications with frameworks like Cordova. Furthermore the Ionic framework builds around create styling that resembles the native platform which makes it 'almost' impossible to tell the difference.
Explain using an example the "fundamentals" of an ionic application.
The fundamentals of Ionic is that its a HTML5 language which builds on AngularJS. 

#####See PhoneApp for example

####Explain using an example how your Hybrid Application communicates with a backend and how CORS problems were solved (if any)
In this example we use Firebase as our backend and thereby simplyfies the process and avoids the CORS problems. 

[See Services.js](www/js/services.js)
