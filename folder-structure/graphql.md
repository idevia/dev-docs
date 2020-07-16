# Guide for folder structure GraphQL

## Nodejs (JavaScript)

You must have to maintain the following folder structure for GraphQL projects

```
root
├── api
│   └── v1
│       ├── controllers
│       │   ├── auth.ctrl.js
│       │   └── users.ctrl.js
│       ├── enums
│       │   ├── statusCodes.js
│       │   └── userRoles.js
│       ├── middleware
│       │   └── auth.middleware.js
│       ├── models
│       │   └── User.js
│       ├── routes
│       │   └── index.js
│       └── utils
│           └── s3-uploads.js
├── app.js
├── db
│   ├── db.js
│   └── seeder
│       ├── index.js
│       └── user.seeder.js
├── lib
│   ├── random-string.js
│   └── utilsLib.js
├── package.json
|── README.md
└── .env
```

## Nodejs (TypeScript)

TBD
