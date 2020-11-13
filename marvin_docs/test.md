## Tests
Aquí se puede detallar / explicar que estrategia vamos a implementar para asegurar que se cumplan con los requerimientos de usuario. Pienso que no sólo abarca Unit Test (Automatizado) sino también procedimientos manuales.

También se puede describir:
* Unit Tests : Priorizando las pruebas unitarias que son esenciales
* Integration Tests

### Smoke Testing Checklist:

- [ ] As a user with a valid email and password | I should be able to login.
- [ ] As a logged in user | I want to upload files in .xls format.
- [ ] As a logged in user | I want to select the model of the files I want to select.
- [ ] As a logged in user with the model selected | I want to see all the files uploaded.
- [ ] As a logged in user with the model selected | I want to select one or more files uploaded.
- [ ] As a logged in user with the model and file(s) selected | I want to see the detail page.
- [ ] As a logged in user in the detail page | I want to see the summary charts (group type and most used tags).
- [ ] As a logged in user in the detail page | I want to use the filters to combine one or more differentiation criteria.
- [ ] As a logged in user in the detail page with the filters activated | I want to see the new summary charts (group type and most used tags).
- [ ] As a logged in user in the detail page with the filters activated | I want to see the benchmark charts (group type and most used tags)
- [ ] As a logged in user in the detail page | I want to download the new file generated that includes the tags, name of the batch and date-time.

### System Testing:
Go to the full document [here](https://docs.google.com/spreadsheets/d/1JfBYyEU9d8gR6bLVPJuSZH48eSpFpgiDtRNKdO-v5DQ/edit?usp=sharing)