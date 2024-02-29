useCases: Coloque os casos de uso do seu aplicativo aqui. Cada caso de uso representa uma funcionalidade específica do seu aplicativo e encapsula a lógica de negócios correspondente.

Example of the code for app/useCases/UserController.ts:
```
import { Request, Response } from 'express';

class UserController {
  getAllUsers(req: Request, res: Response) {
    // Implement logic to retrieve all users
    res.json({ users: [...allUsers] });
  }

  getUserById(req: Request, res: Response) {
    // Implement logic to retrieve a user by ID
    res.json({ user: { id: req.params.id, name: 'John Doe' } });
  }

  createUser(req: Request, res: Response) {
    // Implement logic to create a new user
    res.status(201).json({ message: 'User created successfully' });
  }

  updateUser(req: Request, res: Response) {
    // Implement logic to update a user by ID
    res.json({ message: 'User updated successfully' });
  }

  deleteUser(req: Request, res: Response) {
    // Implement logic to delete a user by ID
    res.json({ message: 'User deleted successfully' });
  }
}

export default new UserController();
```
