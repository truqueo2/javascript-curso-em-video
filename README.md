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

**Formatando string**:
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
Converter string para number:  
```js
    var n = prompt('Digite um numero: ')

    Number.parseInt(n) //converte a string para inteiro
    Number.parseFloat(n) //converte a string para ponto flutuante
    Number(n) //converte a string automaticamente para inteiro ou float
```

## Number

Pode ser **inteiro** ou **ponto flutuante**.

**Formatando number**:  
```js
var n1 = 1543.5
n1.toFixed(2) //fixa duas casas decimais.
n1.toFixed(2).replace('.',',') //replace troca algo por outro, no caso o ponto pela vírgula.

n1.toLocaleString('pt-BR',{style:'currency', currency:'BRL'}) // neste exemplo formata no formato de real.

```

Converter number para string:  
```js
    var n = prompt('Digite um numero: ')

    String(n)
    n.toString()
```

## Operadores

### Aritméticos  
```js
    var x = 5
    var y = 3

    x + y   // soma
    x - y   // subtração
    x * y   // multiplicação
    x / y   // divisão
    x % y   // resto da divisão
    x ** y  // potenciação


/* 
Ordem de Precedência:  
1. ( )  
2. **  
3. * / %  
4. + -  
*/ 
```

### Atribuição

**Atribuição Simples** é representada pelo sinal de igual.  
```js
var a = 5 + 3           //8
var b = a % 5           //8
var c = 5 * b ** 2      //45
var d = 10 - a / 2      //6
var e = 6 * 2 / d       //2
var f = b % e + 4 / e   //3 
```

**Auto-atribuição** é atribuir o valor com o valor dela mesmo e armazena na própria váriavel. Ex:  
```js
    var x = 5;
    var y = 3;

    //forma simplificada        // auto-atribuição
    x += y;                     // x = x + y; soma
    x -= y;                     // x = x - y; subtração
    x *= y;                     // x = x * y; multiplicação
    x /= y;                     // x = x / y; divisão
    x %= y;                     // x = x % y; resto da divisão
    x **= y;                    // x = x ** y; potenciação

```
Incremento e Decremento  

n++  
n--

### Relacionais  

Sempre retorna um valor boolean **true** ou **false**.  
```js
> //maior
< //menor
>= //maio ou igual
<= //menor ou igual
== //igual, não compara o tipo do valor.
!= //diferente

=== //identidade ou igualdade restrita, ele compara o tipo do valor.
!== //desigualdade restrita, verifica tambem se o tipo do valor são diferentes
```

### Lógicos

Sempre retorna um valor boolean **true** ou **false**.  
```js
! //negação (não)
&& //disjunção (e)
|| //conjunção (ou)
```

**Precedencia dos operadores:**  
*Primeiro os aritméticos
*Segundo de comparações
*Terceiros os lógicos e entre os lógicos vem primeiro a **negação**, depois **disjunção** e por último a **conjunção**.

### Ternário
```js
var media = 9.0
//composto por 3 partes

// teste ? true : false
media >= 7.0 ? "Aprovado" : "Reprovado"

//a variável pode receber o valor do teste ternário
var res = media >= 7.0 ? "Aprovado" : "Reprovado"
```

