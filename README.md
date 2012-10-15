#Apigee App Services (Usergrid) Standard jQuery Example

##Overview
This project is a quick example to show how to make App Services (Usergrid) calls with standard [jQuery](http://jquery.com/) ajax calls. Please note that if you are looking for a more comprehensive Javascript SDK that is not platform dependent, please consider our [HTML5 Javascript SDK](https://github.com/apigee/usergrid-javascript-sdk).  

Repo source:

<https://github.com/apigee/Usergrid-jQuery-Example>

To see a live demo of this project:

<http://apigee.github.com/Usergrid-jQuery-Example/>


To find out more about Apigee App Services, see:

<http://apigee.com/about/developers>

To view the Apigee App Services documentation, see:

<http://apigee.com/docs/usergrid/>

##Getting Started
This is a simple project to show how you can use the built-in ajax() method to make calls against the App Services API.  The main file:

js/app.js


The js/app.js file is where all the javascript code resides and where all calls to the API are made. On line 32 of this file, find this code:

	//Your org and app combination - change this!!
	var org = 'apigee'; //<== your organizaiton
	var app = 'sandbox';//<== your application

And put in your account information, so that when you run the app it will connect to the correct account.

The main functions are **get**, **post**, **put**, and **deleteF** (delete is a keyword).  All of these functions take their input and call the **apiRequest** method.  The **apiRequest** method is what actually makes a call to the server.

**Note:** this example uses the "Sandbox" application that comes with your new account.  It does not use authentication tokens, although it could be easily extended to do so as the code to add the token to the header is in the apiRequest method.  

##Known issues
This code (the jQuery ajax function) will not fully work with Internet Explorer < version 10.  In version 10, Microsoft finally implemented XMLHttpRequest which makes all the magic possible. 

##Sample apps
The SDK project includes a simple app called Dogs, that creates a list of dogs.  The app uses App Services to retrieve a collection of dog entities. The app illustrates how to page through the results, and how to create a new entity.

For a more complex sample app, check out the Messagee app:

<https://github.com/apigee/usergrid-sample-html5-messagee>

##More information
For more information on Apigee App Services, visit <http://apigee.com/about/developers>.


## Contributing
We welcome your enhancements!

Like [Usergrid](https://github.com/apigee/usergrid-stack), the Usergrid Javascript SDK is open source and licensed under the Apache License, Version 2.0.

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Added some feature'`)
4. Push your changes to the upstream branch (`git push origin my-new-feature`)
5. Create new Pull Request (make sure you describe what you did and why your mod is needed)


## Copyright

 * Copyright (c) 2012 Apigee, Corp
 *
 * Licensed under the Apache License, Version 2.0 (the "License");
 * you may not use the included files except in compliance with the License.
 * You may obtain a copy of the License at
 *
 *   http://www.apache.org/licenses/LICENSE-2.0
 *
 * Unless required by applicable law or agreed to in writing, software
 * distributed under the License is distributed on an "AS IS" BASIS,
 * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 * See the License for the specific language governing permissions and
 * limitations under the License.ƒ