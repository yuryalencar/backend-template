middlewares: Armazene os middlewares do seu aplicativo aqui. Isso inclui middlewares para autenticação, autorização, manipulação de erros, entre outros.

Example of the code for app/middlewares/authentication.js:
```
const authenticate = (req, res, next) => {
  // Implement authentication logic here
  if (req.headers.authorization === 'Bearer <token>') {
    next();
  } else {
    res.status(401).json({ message: 'Unauthorized' });
  }
};

module.exports = { authenticate };
```
