# Backend folder structure

---

## Example 1

### For smaller projects

This structure is more suitable for smaller projects

```
project
│
│   server.js
│   package.json
│   .env
│   .gitignore
│
└───config
│       │
│       │   passportStrategies.js
│       │   ...
│
└───models
│       │
│       │   UserModel.js
│       │   ...
│   
└───routes
│       │
│       │   user.js
│       │   ...
│   
└───utils
        │
        │   jwtIssuer.js
        │   ...
```

## Example 2

### Separating concerns for larger projects

This example focuses on deep separation of concerns:

- database connection in separate file
- `process.env` variables accumulated in single file - `config.js`

```
project
│
│   server.js
│   package.json
│   .env
│   .gitignore
│
└───config
│       │
│       │   config.js
│       │   database.js
│       │   passportStrategies.js
│       │   ...
│
└───models
│       │
│       │   UserModel.js
│       │   ...
│       │
│       └───schemas
│           │
│           │   UserSchema.js
│           │   ...
│   
└───routes
│        │
│        │   user.js
│        │   ...
│   
└───utils
        │
        │   jwtIssuer.js
        │   ...
```