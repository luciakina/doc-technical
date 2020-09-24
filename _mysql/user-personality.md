#### user_personality

| Field     | Type       | Description                                          |
| :-------- | :--------- | :--------------------------------------------------- |
| id        | int(11)    | Pk                                                   |
| userId    | bigint(20) | Reference to the pk of the user tables               |
| sourceId  | int(11)    | Reference to the sourceId field of the sources table |
| data      | json       | Object returned drom IBM                             |
| createdAt | timestamp  | Creation date                                        |
| updatedAt | timestamp  | Date for last update                                 |
