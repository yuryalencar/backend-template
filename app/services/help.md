Lógica de serviço: Se a lógica de serviço não se encaixa perfeitamente nos casos de uso, ela pode ser mantida aqui. Por exemplo, integrações com APIs externas ou serviços.

Example of the code for services/externalApiService.js:
```
const axios = require('axios');

class ExternalApiService {
  async fetchData() {
    // Implement logic to fetch data from an external API
    const response = await axios.get('https://api.example.com/data');
    return response.data;
  }
}

module.exports = new ExternalApiService();

```
