# Firebase Setup 

When setting up a Firebase project, first start by creating your directory for your project. In that directory, create the following structure:
* dist
    * index.html
* src
    * index.js

You want to run the following command to create the package.json:

`npm init -y`

You then want to install Webpack with the following command:

`npm i webpack webpack-cli -D`

Afterwards, install Firebase with the following command:

`npm i firebase`

Create a file in your main directory called `webpack.config.js`, and copy paste the following:
``` javascript
const path = require('path')

module.exports = {
  mode: 'development',
  entry: './src/index.js',
  output: {
    path: path.resolve(__dirname, 'dist'),
    filename: 'bundle.js'
  },
  watch: true
}
```

In your `package.json` file (which should have been created after installing Firebase), add `"build": "webpack"` to your scripts. Now, when you type the commmand `npm run build` in your console while in the main directory, it should run webpack and create a `bundle.js` file in your `dist` directory. Make sure that your index.html has the following script tag in it's body:

``` HTML
<script src="bundle.js"></script>
```

Now, in your `index.js` file, you need to import the config for your Firebase project. In the Firebase console, go to your Web app's project settings, find **SDK setup and configuration** at the bottom and copy paste the config into your index.js, and import the app. Your `index.js` file should look like the following:

``` javascript
import { initializeApp } from 'firebase/app'

const firebaseConfig = {
  apiKey: "",
  authDomain: "",
  projectId: "",
  storageBucket: "",
  messagingSenderId: "",
  appId: ""
};

// init firebase
initializeApp(firebaseConfig)
```

Now, you should be set up to use Firebase. Remember to import the services that you want to use. 

**There is likely more to set-up, especially with all the other tools and services you can use. So far, this pretty much helps cover Firestore**