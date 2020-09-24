#### personality

| Field        | Type      | Description                                                  |
| :----------- | :-------- | :----------------------------------------------------------- |
| id           | int(11)   | Pk                                                           |
| clientId     | int(11)   | Reference the aq_industry field of the aquiles_clients table |
| intents      | int(11)   | Limit intents                                                |
| intentsCount | int(11)   | Counter intents used                                         |
| lastIntentAt | timestamp | Last intent used                                             |
| status       | boolean   | Status if the client have personality feature                |
| createdAt    | timestamp | Creation date                                                |
| updatedAt    | timestamp | Date for last update                                         |
