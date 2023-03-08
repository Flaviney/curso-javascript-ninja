# Desafio da semana #2

Nesse exercício, você está livre para escolher os nomes para suas variáveis e funções! :smile:

```js
// Crie uma função que receba dois argumentos e retorne a soma dos mesmos.
fuction somar(x,y){
return x + y;
}

// Declare uma variável que receba a invocação da função criada acima, passando dois números quaisquer por argumento, e somando `5` ao resultado retornado da função.
var soma = soma(1,4) + 5;

// Qual o valor atualizado dessa variável?
9

// Declare uma nova variável, sem valor.
var aula2;

/*
Crie uma função que adicione um valor à variável criada acima, e retorne a string:
    O valor da variável agora é VALOR.
Onde VALOR é o novo valor da variável.
*/

function add(x) {
aula2 = x;
return 'O valor da variável agora é ' + aula2;
}

// Invoque a função criada acima.
add(2);

// Qual o retorno da função? (Use comentários de bloco).
/*
O valor da variável agora é 2
*/

/*
Crie uma função com as seguintes características:
1. A função deve receber 3 argumentos;
2. Se qualquer um dos três argumentos não estiverem preenchidos, a função deve retornar a string:
    Preencha todos os valores corretamente!
3. O retorno da função deve ser a multiplicação dos 3 argumentos, somando `2` ao resultado da multiplicação.
*/
function retorna(n1,n2,n3) {
  if (n1 === 0 || n2 === 0 || n3 === 0) {
    return 'Preencha todos os valores corretamente!'
   } else {
    return (n1 * n2 * n3) + 2;
  }
}

// Invoque a função criada acima, passando só dois números como argumento.
retorna(1,2)

// Qual o resultado da invocação acima? (Use comentários para mostrar o valor retornado).

// NaN

// Agora invoque novamente a função criada acima, mas passando todos os três argumentos necessários.
retorna(1,2,3)

// Qual o resultado da invocação acima? (Use comentários para mostrar o valor retornado).
8

/*
Crie uma função com as seguintes características:
1. A função deve receber 3 argumentos.
2. Se somente um argumento for passado, retorne o valor do argumento.
3. Se dois argumentos forem passados, retorne a soma dos dois argumentos.
4. Se todos os argumentos forem passados, retorne a soma do primeiro com o segundo, e o resultado, dividido pelo terceiro.
5. Se nenhum argumento for passado, retorne o valor booleano `false`.
6. E ainda, se nenhuma das condições acima forem atendidas, retorne `null`.
*/
function retorna(n1,n2,n3) {
    if (n1 !== 0 && n2 === 0 && n3 === 0) {
        return n1;
    } else {
        if (n2 !== 0 && n3 === 0 && n1 === 0) {
            return n2;
    } else {
         if (n3 !== 0 && n2 === 0 && n1 === 0) {   
             return n3;
    }
        }
    }

    if (n1 !== 0 && n2 !== 0 && n3 === 0) {
        return n1 + n2;
    } else {
        
        if (n1 !== 0 && n2 !== 0 && n3 !== 0) {
            return (n1 + n2) / n3;
        }
    }
}

// Invoque a função acima utilizando todas as possibilidades (com nenhum argumento, com um, com dois e com três.) Coloque um comentário de linha ao lado da função com o resultado de cada invocação.
retorna(1,0,0) //1
retorna(4,2,0) //6
retorna(4,2,3) //2
