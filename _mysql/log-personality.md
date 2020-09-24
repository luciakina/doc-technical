##### log_personality

| Field             | Type         | Description                                                  |
| :---------------- | :----------- | :----------------------------------------------------------- |
| id                | int(11)      | Pk                                                           |
| clientId          | int(11)      | Reference the aq_industry field of the aquiles_clients table |
| userId            | bigint(20)   | Reference to the pk of the user tables                       |
| sourceId          | int(11)      | Reference to the sourceId field of the sources table         |
| usernameq         | varchar(100) | Username of the user who made the request                    |
| requestAt         | timestamp    | Request date                                                 |
| userPersonalityId | int(11)      | Reference the id field of the user_personality table         |
| status            | varchar(50)  | Request status                                               |
