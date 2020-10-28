## Tests
Aquí se puede detallar / explicar que estrategia vamos a implementar para asegurar que se cumplan con los requerimientos de usuario. Pienso que no sólo abarca Unit Test (Automatizado) sino también procedimientos manuales.

También se puede describir:
* Unit Tests : Priorizando las pruebas unitarias que son esenciales
* Integration Tests

* ### Functional testing:
- [ ] As a user with a valid email and password | I should be able to login.
- [ ] As a logged in user | I should be able to upload files in .xls format.
- [ ] As a logged in user | I should be able to select the model of the files I want to select.
- [ ] As a logged in user with the model selected | I should be able to see all the files uploaded.
- [ ] As a logged in user with the model selected | I should be able to select one or more files uploaded.
- [ ] As a logged in user with the model and file(s) selected | I should be able to see the detail page.
- [ ] As a logged in user in the detail page | I should be able to see the summary charts (group type and most used tags).
- [ ] As a logged in user in the detail page | I should be able to use the filters to combine one or more differentiation criteria.
- [ ] As a logged in user in the detail page with the filters activated | I should be able to see the new summary charts (group type and most used tags).
- [ ] As a logged in user in the detail page with the filters activated | I should be able to see the benchmark charts (group type and most used tags)
- [ ] As a logged in user in the detail page | I should be able to download the new file generated that includes the tags, name of the batch and date-time.