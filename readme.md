
# Rest API file structuring

A brief description of how I structure my APIs

## Main Server Folder

This section shows a structure of the main server folder.

```txt
server/ 📁
└── api/ 📁
  ├── cat/ 📁
  ├── dog/ 📁
  ├── eagle/ 📁
├── utils/ 📁
├── middlewares/ 📁
├── routes.js 📄
└── server.js 📄
```

`api/` - This folder contains the files of an api route.For example, the route `domain.com/api/` will point to that folder.

`api/[Folder]` - This folder is responsible for handling the tasks and of a particular API request. The route `domain.com/api/cat` will be able to access the handler (will be discuessed later) of `api/cat/` folder.

`utils/` - It contains a global functions that can be used for all API routes. 

`middlewares/` - It contains global middlewares.

`routes.js` - It contains all of the route pointing to file.

`server.js` - Handles server configurations

## Contents of API folder

This section contains the utils, middlewares, and helpers of API.

Sample structure

```
server/ 📁
└── api/ 📁
  └── books/ 📁
    ├── books.js 📄
    ├── books.handlers.js 📄
    ├── books.utils.js 📄
    └── books.middlewares.js 📄
...
```

## Definitions

`handlers` - handles a function on how a requests to a specific API route will work.

`utils` - stands for utilities, it contains function definitions that is used on an API

`middlewares` - manages the tools, access, and exposure of an API (examples: isAdmin, isAuthorized)   


## Excerpt

[A future-proof Node.js express file/folder structure](https://www.codemzy.com/blog/nodejs-file-folder-structure)