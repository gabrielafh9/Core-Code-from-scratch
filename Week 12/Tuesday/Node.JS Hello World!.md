# Node.JS Hello World - Practice

## Description

Time to get our hands a little dirty and build our first Node.JS application.

### Practice

0. Open a new command terminal on your computer.
1. Create a new folder in your computer and name it as: ``` hello_world_node ```
2. Go to the folder you just created.
3. Execute the command ``` npm init ``` and answer the question you see in the terminal to create your Node.JS Project
4. Create a new file and name it as: ``` hello_world_node.js ```
5. Make a ``` console.log ``` inside the file with whatever message you want.
6. Run your program by entering the command: ``` node hello_world_node.js. ```

### Analyze Your Practice

0. Why do we run the `npm init` command and not `node init` to create a new Node.JS project?

```
npm init <initializer> can be used to set up a new or existing npm package. 
initializer in this case is an npm package named create-<initializer>, which will be installed by npx, a
nd then have its main bin executed -- presumably creating or updating package.
```

1. When you entered the `npm init` command and answered the questions you saw in the terminal, a new file called `packacke.json` was generated.

- What does this file do?

```
The package.json file provides information such as the name of the project, the version number, a description of the project, the author, and the license. Additionally, it lists all the dependencies that the project needs to run. These dependencies are installed automatically when the project is initialized, using the npm install command. Also, is essential in Node.js development because it makes it easy to manage the project's dependencies and scripts.
```

- Why is this file generated?

```
The package.json file is generated to manage the dependencies and configuration of a Node.js project. It is automatically created when a new project is initialized using the npm init command.

```

### Solution:

[![lunes-node-js.png](https://i.postimg.cc/8cG8fL5R/lunes-node-js.png)](https://postimg.cc/34tfP42N)

[![lunes-node-js-2-0.png](https://i.postimg.cc/NM1StL45/lunes-node-js-2-0.png)](https://postimg.cc/cgLXMxPS)
