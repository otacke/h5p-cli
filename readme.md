An h5p toolkit for running, editing and developing h5p content types.  
Make sure you have [git](https://git-scm.com/downloads), [NodeJS](https://nodejs.org/en/download/current) and [npm](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm) (usually included in NodeJS) installed.  

### INSTALLATION
Uninstall any previous h5p-cli toolkit instance
```
npm uninstall -g h5p-cli
npm uninstall -g h5p
```
then install it from npm
```
npm install -g h5p
```
OR from this repository
```
git clone git@github.com:h5p/h5p-cli.git
cd h5p-cli
npm install
cd ..
npm install -g ./h5p-cli
```

### QUICK START GUIDE
0. `h5p` commands run relative to the current working directory. It's recommended that you run them in a new folder.  
Remember to keep track of your development folders. :)  
1. Install the core h5p libraries.
```
h5p core
```
2. Setup an h5p library like, for example, `h5p-course-presentation`.
```
h5p setup h5p-course-presentation
```
This is required for running and editing content types in the `h5p-course-presentation` library.  
You can install other libraries listed by `h5p list` in the same way.  
For example, `h5p setup h5p-accordion` installs the "h5p-accordion" library and its dependencies.  
`<repoUrl>` is a github repository url. Running the command in this format will also update the library in the local registry. This is useful for unregistered libraries.  
For example, `h5p setup git@github.com:h5p/h5p-accordion.git` installs the "h5p-accordion" library and its dependencies. It also updates its entry in the local library registry.  
[!NOTE]
You can read more on setting up libraries [here](assets/docs/setup.md).  
3. `h5p server` starts the development server.  
You can now use your browser to view, edit, delete, import, export and create new content types.  
4. `h5p help` lists available commands.  
`h5p help <command>` prints the help entry for that `<command>`.  

### Detailed CLI commands

[commands.md](commands.md)
