# Explorify - **A Better Spotify Experience**
# Spotify Accounts Authentication Examples

This project contains basic demos showing the different OAuth 2.0 flows for [authenticating against the Spotify Web API](https://developer.spotify.com/web-api/authorization-guide/).

These examples cover:

* Authorization Code flow
* Client Credentials flow
* Implicit Grant flow

## Installation

These examples run on Node.js. On its [website](https://nodejs.org/en/download) you can find instructions on how to install it. You can also follow this [gist](https://gist.github.com/isaacs/579814) for a quick and easy way to install Node.js and npm.

You need to install Node.js first. Once installed, clone the repository, navigate to the folder and install its dependencies running:

    $ npm install
    
You might also need to install request and request-promise-native npm packages

    $ npm install request
    $ npm install request-promise-native


### Using your own credentials
You will need to register your app and get your own credentials from the Spotify for Developers Dashboard.

To do so, go to your [Spotify for Developers Dashboard](https://beta.developer.spotify.com/dashboard) and create your application. For the examples, we registered these Redirect URIs:

* http://localhost:8888 (For website)
* http://localhost:8888/callback (For Redirect URIs)

Once you have created your app, click on the app that you just created, then click on setting, replace the `client_id`, `redirect_uri` and `client_secret` in the examples `01-fore-explorers/authentication/authentication_code/app.js` with the ones you get from My Applications.

* var client_id = ''; // Your client id
* var client_secret = ''; // Your secret
* var redirect_uri = 'http://localhost:8888/callback'; 


## Running the examples
In order to run the different examples, open the folder with the name of the flow you want to try out, and run its `app.js` file. For instance, to run the Authorization Code example do:

    $ cd authorization_code
    $ node app.js

Then, open `http://localhost:8888` in a browser.
