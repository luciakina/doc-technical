## Data / Schemas Layer

### MongoDB squema

#### Clients
```json
    {
        "_id": {
            "$oid": ObjectID
        },
        "users": [],
        "models": [],
        "name": String,
        "es_index": String,
        "createdAt": {
            "$date": DateTime
        },
        "updatedAt": {
            "$date": DateTime
        },
        "__v": Number
    }
```

#### ConfigModel
```json
    {
        "_id": {
            "$oid": ObjectID
        },
        "filters": [
            {
                "pretty": String,
                "isFilter": Boolena,
                "key": String,
                "type": String
            }, 
            ...
        ],
        "name": String,
        "clientId": {
            "$oid": ObjectID
        },
        "tensorId": {
            "$oid": ObjectID
        },
        "es_index": String,
        "createdAt": {
            "$date": DateTime
        },
        "updatedAt": {
            "$date": DateTime
        },
        "__v": Number
    }
```

### Filters
```json
    {
        "_id": {
            "$oid": ObjectID
        },
        "processId": {
            "$oid": ObjectID
        },
        "createdAt": {
            "$date": DateTime
        },
        "updatedAt": {
            "$date": DateTime
        },
        "__v": 0,
        "filters": {
            [String]: [
                {
                    "key": String,
                    "text": String
                },
                ...
            ],
            ....
        }
    }
```


### Leads
```json
    {
        "_id": {
            "$oid": ObjectID
        },
        "clientId": {
            "$oid": ObjectID
        },
        "processId": {
            "$oid": ObjectID
        },
        "lead": {
            [String]: String | Number | Boolean,
            "labels": [String]
        },
        "createdAt": {
            "$date": DateTime
        },
        "updatedAt": {
            "$date": DateTime
        },
        "__v": Number
    }
```

### Processes
```json
    {
        "_id": {
            "$oid": ObjectID
        },
        "leadsTotal": Number,
        "leadsCount": Number,
        "hasError": Bollean,
        "name": String,
        "fileName": String,
        "configModelId": {
            "$oid": ObjectId
        },
        "clientId": {
            "$oid": ObjectId
        },
        "createdAt": {
            "$date": DateTime
        },
        "updatedAt": {
            "$date": DateTime
        },
        "__v": Number
    }
```

### Tensors
```json
    {
        "_id": {
            "$oid": ObjectID
        },
        "toPredict": [String],
        "y_labels": [String],
        "max_length": Number,
        "name": String,
        "pathPickle": String,
        "pathHdf5": String,
        "pathTdicc": String,
        "createdAt": {
            "$date": DateTime
        },
        "updatedAt": {
            "$date": DateTime
        },
        "__v": Number
    }
```

### Users
```json
    {
        "_id": {
            "$oid": ObjectID
        },
        "permissions": [String],
        "clientId": {
            "$oid": ObjectID
        },
        "userId": ObjectID,
        "username": String,
        "__v": Number
    }
```