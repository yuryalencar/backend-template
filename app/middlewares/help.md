middlewares: Armazene os middlewares do seu aplicativo aqui. Isso inclui middlewares para autenticação, autorização, manipulação de erros, entre outros.

Example of the code for app/middlewares/authentication.ts:
```
import { Request, Response, NextFunction } from 'express';

const authenticate = (req: Request, res: Response, next: NextFunction) => {
  // Implement authentication logic here
  if (req.headers.authorization === 'Bearer <token>') {
    next();
  } else {
    res.status(401).json({ message: 'Unauthorized' });
  }
};

export { authenticate };
```
