## GeradorDeGatinho-API
##### GeradorDeGatinho é uma Mock API DB construida em json-server e hospedada em heroku para armazenar memes de gatinhos que podem ser acessador via fetch preferencialmente por um bot discord. Criei esta API para utilizá-la em meu outro projeto, o discord bot "senjougahara". 

##### Caso possua interesse de uso:
```
GET https://geradordegatinhosapi.herokuapp.com/gatinhos/
```
##### usando node-fetch:
```
const fetch = require('node-fetch')

const response = await fetch(https://geradordegatinhosapi.herokuapp.com/gatinhos/);
const data = await response.json();

console.log(data);
```

##### usando axios
```
const axios = require('axios');

axios.get('https://geradordegatinhosapi.herokuapp.com/gatinhos/')
    .then(resp => {
        data = resp.data;
        console.log(data);
    })
    .catch(error => {
        console.log(error);
    });
 ```
