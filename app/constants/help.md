Armazene constantes que são usadas em várias partes do código. Isso pode incluir códigos de status HTTP, mensagens de erro, etc.

Example of the code for constants/httpStatus.js:
```
const HTTP_STATUS = {
  OK: 200,
  CREATED: 201,
  UNAUTHORIZED: 401,
  // Add more HTTP status codes as needed
};

module.exports = HTTP_STATUS;
```
