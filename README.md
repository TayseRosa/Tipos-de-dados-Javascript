<h1 align="center"> Javascript - Funções de array map(), filter(), reduce(), every(), some(), find(), includes()</h1>

#Índice
- [🛠 Sobre o projeto](#-sobre-o-projeto)
  - [Exemplo de map()](#exemplo-de-map)
  - [Exemplo de filter()](#exemplo-de-filter)
  - [Exemplo de Reduce()](#exemplo-de-reduce)
  - [Exemplo de Every()](#exemplo-de-every)
  - [Exemplo de some()](#exemplo-de-some)
  - [Exemplo de find()](#exemplo-de-find)
  - [Exemplo de includes()](#exemplo-de-includes)
- [🚀 Tecnologias utilizadas neste projeto](#-tecnologias-utilizadas-neste-projeto)
- [📥 Como usar](#-como-usar)
- [🚀 Autor](#-autor)
  
---
# 🛠 Sobre o projeto

<p>Estudo sobre funções de array com Javascript</p>

push - Insere mais um dado no array 
pop - Remove um dado do array

## Exemplo de map()
index.html
```js
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body style="background-color: #121212">
    <h1 style="color:#fff">Funções de array JS</h1>

    <script src="script.js"></script>
</body>
</html>
```

script.js
```js
/*======================================================
 Map() -  map nao altera o array original, ele cria um novo array com as modifiaçoes
 =======================================================*/
const numbers = [1,2,4,5,10];
const dobraValores = numbers.map(  num => num * 2);
console.log( dobraValores );
```

## Exemplo de filter()
script.js
```js
/*======================================================
 Filter() - Remover elementos indesejados com base em condições
 =======================================================*/
const numbers2 = [ 2,3,4,5,4,12,19,7,2,5 ]
const arrayFiltrado = numbers2.filter( (elem, index, arr) => arr.indexOf(elem) === index ) //Esta eliminando valores repetidos
console.log(arrayFiltrado)

```
## Exemplo de Reduce() 
script.js
```js
/*======================================================
 Reduce() - Encontrar um valor cumulativo concatenado, com base em elementos de todo o array
 =======================================================*/
const rockets = [
    {country: 'Russia', launches:32},
    {country: 'US', launches:23},
    {country: 'China', launches:16},
    {country: 'Europe', launches:7},
    {country: 'India', launches:4},
    {country: 'Japan', launches:3},
]

const totalLaunches = rockets.reduce( (prevVal, elemAtual) => prevVal + elemAtual.launches, 0) /* descobrir o total de lançamentos de todos os paises */
console.log(totalLaunches);

```


## Exemplo de Every()
script.js
```js
/*======================================================
 Every() - Testar se todos os elementos de um array 'passam' por um teste especifico(muito parecido com o filter, mas o filter retorna um novo array objeto, mas o every vai dar um resultado booleano)
 =======================================================*/
 /* Verificar se todos os elementos de um array sao maiores que 10 */
 const numbers3 = [ 2,3,4,5,4,12,19,7,2,5 ]
 const saoMaioresQue10 = numbers3.every( elem => elem >= 10 )
 console.log(saoMaioresQue10)

```

## Exemplo de some()
script.js
```js
/*======================================================
 Some() - Quando é preciso testar se pelo menos um elemento do array passa por um teste específico - Retorna true ou false
 =======================================================*/
 /* Verificar se há um numero primo */
 function isPrime( value ){
     for(let i=2; i<value; i++){
         if(value % i === 0 ){
             return false;
         }
     }
     return value > 1
 }

const numbers4 = [ 6,8,11,14,42 ]
const primoOuNao = numbers4.some( (isPrime) )
console.log( primoOuNao )

```

## Exemplo de find()
script.js
```js
/*======================================================
 Find() - Encontrar um valor dentro de um array/objeto, sendo que esse retorno sera do primeiro elemento que satisfizer o teste
 =======================================================*/
 const pizza = ['marguerita', 'mussarela', 'calabreza', 'frango catu' ];
 const encontrarPrimeiraPizzaComM = pizza.find( p => p.startsWith('m') );
 console.log(encontrarPrimeiraPizzaComM)

```

## Exemplo de includes()
script.js
```js
/*======================================================
 Includes() - Encontrar um valor dentro de um array/objeto, sendo que esse retorno sera do primeiro elemento que satisfizer o teste - Diferença em relação ao find, é que ele retorna BOOLEANO.
 =======================================================*/
 console.log( [1,2,3].includes(2) );

```


# 🚀 Tecnologias utilizadas neste projeto

- [x] JAVASCRIPT

# 📥 Como usar
```js

    //Clonar o repositório
    $ git clone https://github.com/TayseRosa/Tipos-de-dados-Javsacript.git

    //Entrar no diretório
    $ cd Tipos-de-dados-Javsacript

    //Rodar projeto
    Duplo clique em index.js e verificar no console do navegador.

``` 

# 🚀 Autor

<a href="https://www.tayserosa.dev">
 <img style="border-radius: 50%;" src="https://avatars.githubusercontent.com/u/31596454?v=4" width="100px;" alt="Tayse Rosa" style="border-radius:50%"/>
 <br />
 <sub><b>www.tayserosa.dev</b></sub></a> <a href="https://www.tayserosa.dev" title="Tayse Rosa" target="_blank">🚀</a>


Feito com ❤️ por Tayse Rosa 🚀

👋🏽 Entre em contato!

![Linkedin Badge](https://img.shields.io/badge/-TayseRosa-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/tayse-rosa-3b683151/)[![GitHub Badge](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/TayseRosa/)
