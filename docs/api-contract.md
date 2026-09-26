Курс: Б1.В.ДЭ.01.02.02 · КГЭУ · семестр 1 · 2026/2027  
Студент: Карамов Марсель Айратович · Группа: ТРИС-3-23 · Дата: 26.09.2026

# Таблица API

| Метод | Путь                              | Тело                                                        | Успех                            | Возможная ошибка |
| ----- | --------------------------------- | ----------------------------------------------------------- | -------------------------------- | ---------------- |
| GET   | /api/applications                 | —                                                           | 200, массив заявок или []        | —                |
| GET   | /api/applications/{id}            | —                                                           | 200, объект заявки               | 404              |
| POST  | /api/applications                 | title, description, postId, departmentId                    | 201, id, number, status: New 400 | 400              |
| PATCH | /api/applications/{id}/hr         | hrId                                                        | 200, обновлённая заявка          | 404, 409         |
| PATCH | /api/applications/{id}/tech       | techId                                                      | 200, обновлённая заявка          | 404, 409         |
| PATCH | /api/applications/{id}/status     | status                                                      | 200, обновлённая заявка          | 404, 409         |
| GET   | /api/applications/{id}/history    | —                                                           | 200, массив записей истории      | 404              |
| GET   | /api/applications/{id}/interviews | —                                                           | 200, массив собеседований        | 404              |
| POST  | /api/applications/{id}/interviews | interviewerUserId, scheduledAt, conductedAt,result, comment | 201, объект собеседования        | 400, 404         |
| GET   | /api/posts                        | —                                                           | 200, массив должностей           | —                |
| GET   | /api/departments                  | —                                                           | 200, массив подразделений        | —                |
| GET   | /api/users?role=HRSpecialist      | —                                                           | 200, массив пользователей        | —                |
| POST  | /api/auth/login                   | login, password                                             | 200, токен и роль                | 401              |
