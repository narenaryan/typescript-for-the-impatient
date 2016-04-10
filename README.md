# Type Script for the Impatient 

Typescript is a transpiling language which generates the plain JavaScript. TypeScript is used to enforce type system to catch many errors at compile time. It also allows us to build Object Oriented designs with little effort. Programmers coming from background of .NET or Java can easily adopt Type Script. Coders of scripting style will learn design patterns by using Type Script. With this book one can easily jump-start coding in typescript.

## Installing Node and Type Script
First in order to proceed, we should install both NodeJS and TypeScript to experiment. so if you are on Ubuntu Machine just install node using this command.

Installing Node and NPM

```
$ sudo apt-get update
$ sudo apt-get install nodejs && sudo apt-get install npm
$ sudo npm install -g n && sudo n stable
```

Installing the TypeScript via NPM


```
$ npm install -g typescript
```

That's it. We are ready with the setup. We are not going to use any IDE here. If you wan't to then chose Brackets with TypeScript plugin. It has very good properties of hinting, warnings etc. 

## Hello World
/* hello_world.ts */

```
  console.log("Hello World");
  
```
### compiling a typescript file
```
$ tsc hello_world.js
```
This line generates a plain JavaScript file and now we can execute it using node.
```
$ node hello_world.js
```