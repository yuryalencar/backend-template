Funções utilitárias: Armazene funções utilitárias reutilizáveis que podem ser usadas em diferentes partes do seu código.

Example of the code for utils/dateUtils.js:
```
const getCurrentDate = () => new Date().toISOString();

module.exports = { getCurrentDate };
```
