Constantes do aplicativo: Armazene constantes que são usadas em várias partes do código, como códigos de status HTTP, mensagens de erro, etc.

Example of the code for config/appConfig.js:
```
const appConfig = {
  port: process.env.PORT || 3000,
  environment: process.env.NODE_ENV || 'development',
  // Add other application-specific configurations here
};

module.exports = appConfig;
```
