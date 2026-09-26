# Матрица требований

| Требование ЛР1        | Поле или сущность                                     | Запрос                              | Критерий |
| --------------------- | ----------------------------------------------------- | ----------------------------------- | -------- |
| Создать объект        | Application, title, description, postId, departmentId | POST /api/applications              | 1        |
| Назначить исполнителя | Application.hrId                                      | PATCH /api/applications/{id}/hr     | 2        |
| Назначить исполнителя | Application.techId                                    | PATCH /api/applications/{id}/tech   | 2        |
| Перевести в работу    | Application.status                                    | PATCH /api/applications/{id}/status | 3        |
