Grunt is a JavaScript task runner that facilitates the development process of an application. There are many tasks during the development of an application that a developer has to do manually. For instance, after each change to the source code, the developer has to refresh the web browser to see the effects of the changes. Other examples of this are the process of concatinating files, minifying files or running unit tests, which often have to be directly initated by developers. 

It can accomplish automation with one command.

Grunt automates these repetitive and mundane tasks, saving the developer valuable time that can go into the actual building of the application. 

In Grunt, the automation of tasks is configure in one file, the Gruntfile.js. 

Your gruntfile should be in the directory where you run the grunt command.

Grunt runs in the Node.js platform, so you must have Node installed on your machine. 

The most common use of Grunt is the build process. 

1. download tasks 
2. import tasks so that you can use them
3. you then define options and settings on tasks
4. you can run that task in the command line
5. or you can register it as one of several tasks

What is the Grunt file?

Gruntfile.js is your configuration for grunt. This is where you tell grunt what plugings you want to use and with what settings. It's where the magic happens. 

grunt --help
grunt --help -verbose
grunt jshint

What are Grunt plug ins?

Contrib plugins are done by the grunt team
npm install grunt-contrib-jshint --save-dev

Grunt tasks need a configuration object

Installing Grunt 

1. 'npm install -g grunt cli'

2. in your program locally -> 'npm install grunt --save-dev', this adds grunt as a devDependency 

3. create a Gruntfile.js

module.exports = function(grunt) {
	grunt.initConfig({ //object that configures how grunt is going to run


	})
	grunt.registerTask("default", function(name){ //default task, runs with 'grunt' command in cli
													//grunt default:Carlos -> you can pass in parameters		
		grunt.log.writeln("Hello world!")
	})
}

Running Grunt
Each time grunt is run, it looks for a locally installed Grunt using node's require() system. Because of this, you can run grunt from any subfolder in your project.

If a locally installed Grunt is found, the CLI loads the local installation of the Grunt library, applies the configuration from your Gruntfile, and executes any tasks you've requested for it to run. 

