endpoints: Este diretório pode conter módulos ou arquivos que lidam com as rotas da sua aplicação, definindo os pontos finais da API e chamando os controladores correspondentes.

Example of the code for app/endpoints/users.js:
```
const express = require('express');
const router = express.Router();
const UserController = require('../useCases/UserController');

router.get('/', UserController.getAllUsers);
router.get('/:id', UserController.getUserById);
router.post('/', UserController.createUser);
router.put('/:id', UserController.updateUser);
router.delete('/:id', UserController.deleteUser);

module.exports = router;
```
