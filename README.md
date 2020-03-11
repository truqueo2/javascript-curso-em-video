# javascript-curso-em-video

## Variáveis e Tipos Primitivos

Para declarar a variável é só usar as palavras reservadas **var**, **let** ou **const**.

**Identificadores**:  
*Podem começar com **letra**, **$** ou **_**  
*Não podem começar com **números**  
*É possível usar **letras** ou **números**  
*É possível usar **acentos** e **símbolos**  
*Não podem conter **espaços**  
*Não podem ser **palavras reservadas**  

**Tipos Primitivos**:  
*number  
**Infinity  
**NaN  
*string  
*boolean  
*null  
*undefined  
*objetct  
**Array  
*function  

Para saber o tipo primitivo é só usar o comando **typeof** e o nome da variável ou declaração literal.

ex:  
```js
var n = 20  

typeof n //number  
typeof 20  //number  
```

## String

```js
var nome = 'Jhonny' //usando aspas simples
var sobrenome = "Oliveira" //usando aspas dupla
var sexo = `masculino` //usando crase, chamado de template string
```

Formatando string:
```js
    var nome = 'Jhonny'
    var sobrenome = "Oliveira"
    var sexo = `masculino`

    document.write('O meu nome é ' + nome + ' ' + sobrenome + ' e sou do sexo ' + sexo) // concatenação
    document.write("O meu nome é " + nome + " " + sobrenome + " e sou do sexo " + sexo) // concatenação
    document.write(`O meu nome é ${nome} ${sobrenome} e sou do sexo ${sexo}`) // template string

    nome.length // tamnho da string
    nome.toUpperCase() // tudo maiusculo
    nome.toLowerCase() // tudo minusculo
```
