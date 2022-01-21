
# Xero Java oAuth2 Starter
This Java project contains the code necessary to use the Xero-Java SDK and complete OAuth 2 flow

Note: this project was built & tested using [Visual  Studio Code](https://code.visualstudio.com/) and [Apache Tomcat 9.x](http://tomcat.apache.org/) server.

## Create a Ledgerflow App
To obtain your API keys, follow these steps and create a Ledgerflow app

* Create a [free Ledgerflow user account](https://flow.ledgerscope.com/Account/Register)
* Login to your Ledgerflow developer [dashboard](https://flow.ledgerscope.com/Partner/App) and create an API application
* Copy the credentials from your API app and store them using a secure ENV variable strategy
* Decide the [neccesary scopes](https://developer.xero.com/documentation/oauth2/scopes) for your app's functionality

## Add your API keys to this app
You'll need to set the *clientId, clientSecret and redirectURI* in the following files

* Authorization.java
* Callback.java
* TokenRefresh.java

You also need to replace --SOURCE ACCOUNTING SOFTWARE--.
The source accounting software values are 1004 to return QuickBooks Online data and 1009 to return Sage Business Cloud Accounting data.

## Build and deploy
Compile your app and deploy to a server (tomcat, etc)
```sh
mvn clean install
```

Deploy on Tomcat or other Java server.

## License

This software is published under the [MIT License](http://en.wikipedia.org/wiki/MIT_License).

	Copyright (c) 2019 Xero Limited

	Permission is hereby granted, free of charge, to any person
	obtaining a copy of this software and associated documentation
	files (the "Software"), to deal in the Software without
	restriction, including without limitation the rights to use,
	copy, modify, merge, publish, distribute, sublicense, and/or sell
	copies of the Software, and to permit persons to whom the
	Software is furnished to do so, subject to the following
	conditions:

	The above copyright notice and this permission notice shall be
	included in all copies or substantial portions of the Software.

	THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
	EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
	OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
	NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
	HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
	WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
	FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
	OTHER DEALINGS IN THE SOFTWARE.