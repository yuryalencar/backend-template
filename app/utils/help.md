Funções utilitárias: Armazene funções utilitárias reutilizáveis que podem ser usadas em diferentes partes do seu código.

Example of the code for utils/dateUtils.ts:
```
const getCurrentDate = (): string => new Date().toISOString();

export { getCurrentDate };
```
