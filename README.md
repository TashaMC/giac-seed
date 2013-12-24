giac-seed 
(grunt-ionic-angular-cordova seed)
=========

The alternative starter template for ionic-angular project (http://ionicframework.com/) for Cordova with Grunt automatization.

Installation
=========

1. Create your cordova app with [Cordova CLI](http://cordova.apache.org/docs/en/3.3.0/guide_cli_index.md.html#The%20Command-Line%20Interface)
<pre><code>
cordova create my-cordova-project com.example.mycordovaproject MyCordovaProject
</code></pre>
Don't forget paste next lines in ```www/config.xml``` file
<pre><code>
<preference name="webviewbounce" value="false" />
<preference name="UIWebViewBounce" value="false" />
<preference name="DisallowOverscroll" value="true" />
</code></pre>
2. Install [grunt-cli](http://gruntjs.com/getting-started#installing-the-cli)
<pre><code>
npm install -g grunt-cli
</code></pre>
3. Install [compass](http://compass-style.org/install/)
<pre><code>
gem install compass
</code></pre>
4. Download and unzip content of giac-seed-master folder into cordova project folder to get a structure like this:
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

1. Write your code in ```giac``` folder. There is a basic project template:
<pre><code>giac/
├── css/           
├── fonts/
├── img/
├── js/
    ├── lib/       // <!-- set of needed ionic and angular js libraries -->
    └── app.js     // <!-- place for your JS code -->
├── scss/
    ├── iconic/
    └── app.scss   // <!-- place for your SASS code -->
└── index.html     // <!-- plase for your HTML code -->
</code></pre>  
2. Compile your code by simply typing ```grunt``` in command line.
<pre><code>
cd my-cordova-project
grunt
</code></pre>
This operation will replace all content of ```my-cordova-project/www``` except of ```confifg.xml``` file with minified application files that compiled from ```giac``` source.
3. To deploy app onto device use Cordova as usually.

Tips
=========

1. You can work in "real-time" mode using NetBeans or JetBrains connector navigating ```giac/index.html``` page.
2. Only minimal set of angular libraries are included. They are ```angular.js```, ```angular-animate.js```, ```angular-route.js```, ```angular-sanatize.js```, ```angular-touch.js```. If you need more ```angular-*.js``` files, put them into ```giac/js/lib/angular``` folder and include into ```giac/index.html``` between ```<!-- GIACSTART --><!-- GIACEND -->``` tags.

TODO
=========

1. Put all needed files (```node_modules``` etc.) into ```giac``` folder.
2. Add some testing modules (jasmine).
