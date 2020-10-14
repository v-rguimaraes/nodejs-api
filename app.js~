

const express = require('express')
const app = express()


app.get("/numrandom", (request, response) => {

    const min = Math.ceil(1000);
    const max = Math.floor(9999);
    let numPedido = Math.floor(Math.random() * (max - min + 1)) + min;
  
    //response.send(numPedido.toString())
    
    //p78f5de44db7ae777f514
    const crypto = require("crypto");
    const strPedido = 'p'+crypto.randomBytes(10).toString('hex');
    response.send('O código gerado para voce foi-->'+strPedido)

});

app.get('/', (request, response) => {

    response.send('Bem Vindo a Nossa API')

})

app.listen( 8080, () => {
  console.log(`API Ouvindo na Porta 8080`)
})