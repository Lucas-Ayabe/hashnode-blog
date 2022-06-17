## Aprendendo orientação a objetos I - paradigmas de programação

Aprender o paradigma orientado a objetos não é algo fácil, e eu sempre percebi que esse era um assunto complicado de entender pelas pessoas com o qual eu interajo, por isso resolvi criar essa série de artigos dando a minha visão de como aprender esse assunto tão requerido hoje em dia e espero poder ajudar a você que doou o seu tempo vindo ler o meu blog.
# Introdução
Nessa série eu gostaria de começar explicando o que são paradigmas de programação, afinal a orientação a objetos é um paradigma de programação, então acredito que começar explicando o que é isso possa ajudar.

Muitas pessoas começam a aprender como programar com a tal da lógica de programação, e depois seguem aprendendo sobre a OOP (Object Oriented Programming, ou traduzindo: programação orientada a objetos) pensando nela como uma evolução do que elas haviam aprendido antes.

O que é uma conclusão um tanto quanto equivocada, o que as pessoas aprendem como lógica de programação é simplesmente um outro paradigma de programação: o procedural.

# O que é um paradigma de programação
Para entendermos o porquê de ser uma conclusão um tanto quanto equivocada, precisamos entender o que é um paradigma de programação, que em uma definição simples seria: o jeito que nós utilizamos para resolver um problema quando vamos programar uma solução para ele.

> Paradigmas de programação são jeitos de classificar linguagens de programação baseado nas suas funcionalidades.

> *~ [Wikipedia](https://en.wikipedia.org/wiki/Programming_paradigm) (Tradução livre)*

Com esse trecho fica claro que necessariamente um paradigma não torna uma linguagem melhor ou pior, é simplesmente uma forma de nós classificarmos que tipo de funcionalidades nós esperamos encontrar nelas. E essas funcionalidades podem ser melhores ou piores dependendo do problema que estamos tentando resolver.

# Principais paradigmas de programação
Atualmente os 3 paradigmas mais populares de programação são:
- Procedural (organiza as instruções do programa em procedimentos ou funções);
- Orientado a objetos (organiza as instruções junto aos dados em que elas operam na forma de objetos);
- Funcional (organiza as instruções como funções puras);

E eles são subdivisões dos paradigmas:
- Imperativo (você diz para o computador como alterar o seu estado até chegar ao resultado final, semelhante a uma receita);
- Declarativo (você diz para o computador quais transformações ele deve aplicar para chegar no resultado final);

## Programação imperativa
Para entendermos melhor a diferença entre essas duas categorias, na programação imperativa você programa da forma que geralmente se é ensinado, pensando no seu algoritmo como uma série de instruções para se chegar em um resultado final, como uma receita. Por exemplo:
```javascript
var x = 1;
x = x + 1;

console.log(x); // 2
```

Nesse simples programa primeiro nós dizemos que o estado dele é o número 1, pois nós criamos uma variável `x`, depois nós dizemos que o computador deve incrementar o valor dela em 1, e atribuir esse valor incrementado a própria variável `x` dessa forma, efetivamente alterando o estado do nosso programa.
Para verificar isso nós mostrados o valor de `x` após ele ser atualizado através do comando `console.log` (o trecho de código é escrito em JavaScript, e `console.log` é um comando para mostrar algo no console).

## Programação declarativa
Do outro lado, quando falamos de programação declarativa, nós descrevemos como nós queremos que seja o resultado final do nosso programa, seria algo como:
```javascript
const incrementedByOne = x => x + 1;
console.log(incrementedByOne(1));
```

Observe que embora o resultado final tenha sido o mesmo, nesse caso ao invés de representar nosso programa como um estado inicial que é modificado até chegar ao resultado esperado, aqui nós descrevemos que computação queremos que seja feita (na forma de uma função chamada `incrementedByOne`, que é nomeada com a intenção de representar o resultado dela ao invés da ação que ela realiza) de forma a representar o nosso estado final.

# Conclusão
Este artigo tem a ideia de te introduzir ao que é um paradigma de programação então não se preocupe se não entender 100%, pois é um assunto realmente extenso. A partir daqui nós iremos dar um passo para trás e falar um pouco sobre a programação procedural em nosso [próximo artigo](https://hashnode.com/draft/62abede22b2b09182b657657) para ai sim conseguirmos entender a necessidade de programarmos de forma orientada a objetos, espero que você que leu até aqui tenha se interessado e que goste desse e dos próximos artigos dessa série.