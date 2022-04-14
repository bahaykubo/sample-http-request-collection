# Http Requests Collection with Thunder Client

This is a collection of http requests using [Thunder Client](https://www.thunderclient.com/) as a VS Code extension. In addition to having our http request client as an extension of our IDE and not requiring to install a separate application, this allows us to easily version control our collections and collaborate and share across the team.

- [Http Requests Collection with Thunder Client](#http-requests-collection-with-thunder-client)
  - [Install Thunder Client](#install-thunder-client)
  - [Using Thunder Client](#using-thunder-client)
    - [Activity](#activity)
    - [Collection](#collection)
    - [Environment](#environment)
    - [Sharing](#sharing)
    - [Opening Other Thunder Client Projects](#opening-other-thunder-client-projects)

## Install Thunder Client

Thunder client runs as an extension of VS Code. so it's required to have vs code installed first. [Get and install vs code first](https://code.visualstudio.com/download).

Once installed, run the following to install the thunder client extension:

```bash
code --install-extension rangav.vscode-thunder-client
```

You should then get the thunder client extension icon available from the activity bar.

## Using Thunder Client

Watch this short clip to [see how Thunder Client works](https://www.youtube.com/watch?v=NKZ0ahNbmak&t=3s&ab_channel=ThunderClient).

And see this [documentation from the thunder client github project](https://github.com/rangav/thunder-client-support) for information on how to use thunder client. There are further information about each component of it below. 

### Activity

Activities tracks a history of any `request` that was created or sent in thunder client. As soon as a new request is created, this gets recorded as an `Activity`. From the Activity tab, you can then pick and choose any request to be added to a collection.

We do not keep track of your local activity in our source control. If there is a request that is to be shared across, this needs to be added to a collection.

### Collection

Collections are groups of requests that are available and source controlled by this project. Anyone that clones this project will have access to requests from these collections. And any contributor can commit creation, update and deletion of requests on any collection that are available from this project. 

### Environment

Environments are collections of key-value pairs that can be accessed as variables from any requests. There can only be one active `Environment` at a time.

To reference a variable, you will use two opening and closing brackets ie `{{variableName}}`.

### Sharing

This project keeps track of collection requests and environments only. Your local activity is not tracked and will not be shared and available to anyone who clones or have access to this project.

If you need a request to be shared, you will need to add this to an existing collection, or create a new collection and add this request to it.

### Opening Other Thunder Client Projects

Thunder Client will pick up this project as it's context for diplaying collections and environments if VS Code has this project open. If you have another Thunder client "project", you can use this "project" as the context of Thunder Client by either opening this project's directory from a new instance of VS Code or in an existing VS Code instance.
