# Guide for folder structure GraphQL

## Nodejs (JavaScript)

TBD

## Nodejs (TypeScript)

You must have to maintain the following folder structure for GraphQL projects

```
server
├── app
│   ├── index.ts
│   └── v1
│       ├── interfaces
│       │   └── User.ts
│       ├── models
│       │   ├── User.ts
│       │   └── index.ts
│       ├── resolvers
│       │   ├── index.ts
│       │   └── userResolvers.ts
│       └── typeDefs
│           ├── index.ts
│           ├── query.ts
│           └── types
├── index.ts
├── nodemon.json
├── package.json
└── tsconfig.json
```
