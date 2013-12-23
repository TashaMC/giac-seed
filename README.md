giac-seed (grunt-ionic-angular-cordova seed)
=========

The alternative starter template for ionic-angular project (http://ionicframework.com/) for Cordova with Grunt automatization.

Installation
=========

1. Create your cordova app with [Cordova CLI]
(http://cordova.apache.org/docs/en/3.3.0/guide_cli_index.md.html#The%20Command-Line%20Interface)
```
cordova create my-cordova-project com.example.mycordovaproject MyCordovaProject
```
2. Install [grunt-cli]
(http://gruntjs.com/getting-started#installing-the-cli)
```
npm install -g grunt-cli
```
3. Download and unzip content of giac-seed-master folder into cordova project folder to get those structure:
<pre><code>my-cordova-project/
├── giac/
├── merges/
├── node_modues/
├── platforms/
├── plugins/
├── www/
├── README.md
├── package.json
├── LICENSE
└── Gruntfile.js
</code></pre>

Usage
=========

1. Write your code in giac folder. There is a basic project template with next structure:  
js/app.js - your JavaScript source code
sass/app.scss - your SASS source code
js/lib/** - included Ionic JavaScript files
js/lib/angular/** - minimal set of AngularJS files (you can add more if you need)
index.html - HTML source file (entry point). You can observe it in browser
2. Compile your code by simply typing "grunt" in command line. After that you will get minified code (and sass->css to) in your www folder.

Sorry, have no time - will write it tomorrow

