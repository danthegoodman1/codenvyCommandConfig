# CodenvyCommandConfig
Quick config for running Run commands on Codeenvy

### Once you create the workspace:
1. Make a project
2. In the top right where it says: 
>**Ready** - start command

Click on it and select create new command. That will take you into the run command editor.

3. Follow the instructions below:

### "Command Line"
You start in the /projects folder, which is the parent folder for all projects.

If I wanted to run `hello.js` in the `testProj` project, I would have the command:

`node testProj/hello.js`

### Preview URL
*Make sure that the project you want to run is enabled if you want it to be internet exposed*

`http://${server.port.8080}`

I used that to expose an express server running on port 8080 to the internet.

### Once you have created the command by saving it:
Select the command by hitting the drop down arrow next to the play button in the top middle, select the command, and then you can fetch the preview URL to access it. You can get the actual URL that your project will be running on by running the command, then clicking the button in the very top right and clicking the one that says:

`dev-machine:$PORT` where `$PORT` is the port you are running your service on. That will take your browser to the link that the app is running on and will continue to be that link until you stop the workspace.

### Other notes about Codevny:
- On macOS, using option works for deleting and moving by word, but using command only works for moving by line, not deleting line
- Can use Command-S to save on macOS
- Workspaces timeout after 10 minutes for the free version
- Attempting Local IDE Mount/Sync can be found [here](https://codenvy.com/docs/user-guide/sync/index.html)
- By going into a workspace's settings, you can share the workspace with other people. I don't think you can see the same terminal, but you can watch each other code in close to real time.
- Team workspaces seem to be broken af right now, but normal sharing works fine
- Codenvy saves files as you edit them (automatically), so hitting command-s on normal files don't do much except force the save then and there (maybe you are faster than the system that determines whether to save or not idk)
