## Data / Schemas Layer

### MongoDB squema

```json
    {
        email: {
            type: String,
            required: true,
        },
        password: {
            type: String,
            required: true,
        },
        username: {
            type: String,
            required: true,
        },
        permissions: {
            type: [String],
        },
        groupId: {
            type: Number,
        },
        clientIds: {
            type: [Number],
        }
    }
```
