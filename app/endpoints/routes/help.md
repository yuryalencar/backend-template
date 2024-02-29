endpoints: Este diretório pode conter módulos ou arquivos que lidam com as rotas da sua aplicação, definindo os pontos finais da API e chamando os controladores correspondentes.

Example of the code for app/endpoints/users.ts:
```
import { Router } from 'express';
import UserController from '../useCases/UserController';

const router = Router();

router.get('/', UserController.getAllUsers);
router.get('/:id', UserController.getUserById);
router.post('/', UserController.createUser);
router.put('/:id', UserController.updateUser);
router.delete('/:id', UserController.deleteUser);

export default router;
```
