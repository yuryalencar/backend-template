tests: Mantenha os testes da sua aplicação neste diretório. Use estruturas como Mocha, Jest ou outros frameworks de teste para organizar e executar seus testes.

Example of the code for app/tests/user.test.ts:
```
import request from 'supertest';
import app from '../app'; // Assuming your app is configured in this file

describe('User Endpoints', () => {
  it('should get all users', async () => {
    const res = await request(app).get('/users');
    expect(res.statusCode).toEqual(200);
    expect(res.body).toHaveProperty('users');
  });

  // Add more test cases for other endpoints
});
```
