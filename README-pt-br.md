# Guia Prático: Vibe Coder sem Quebrar a Aplicação

## INTRODUÇÃO

O propósito desse repositório é ensinar como codar chegando o mais próximo possível de um "vibe coder" sem quebrar sua aplicação. O pulo do gato aqui é tentar achar o meio termo entre "vibe coding flow" e "codagem raiz". Para isso, você precisará:

1. Prompts bem feitos
2. Contextos pequenos
3. Escrever seu plano em "pseudocódigo" da maneira mais simples possível

## PROMPT BEM FEITO

Um prompt bem feito é aquele que diz exatamente a entrada, saída e demonstrar informações relevantes para a IA. Exemplo:

> "Tenho isso aqui que funciona assim..."  
> "Quando eu fazer X, quero que o resultado seja Y".

Prompts bem feitos fazem a IA ser bem específica, diminuindo e muito a chance de delírios, gambiarras e afins.

## CONTEXTO PEQUENO

Para aumentar cada vez mais a chance da IA dar boas soluções e não viajar é importante resolver em partes. Aqui irá treinar uma habilidade fundamental: resolver as coisas em pequenas partes. Podem acontecer dois problemas aqui:

### 1) Ficar perdido e não souber dividir

Isso terá que resolver com treino e também pedindo ajuda para a IA.

### 2) O problema DEFINITAMENTE não tem como dividir em um contexto pequeno

Este é mais complicado. O que recomendo é ir anotando trechos do contexto para entender o geral. Por exemplo, as vezes terá que pesquisar em vários arquivos para entender o que está acontecendo. Pode fazer assim:

- O Arquivo X declara ou recebe uma variável
- Essa variável vem do Arquivo Y (via função, import, service, etc.)
- No Arquivo Y, essa variável é usada para executar alguma operação (ex: query no banco)
- O banco retorna um resultado
- Esse resultado volta para o Arquivo Y, possivelmente tratado ou transformado
- Depois retorna para o Arquivo X, onde é finalmente usado (renderização, regra de negócio, etc.)

Aqui você tem uma árvore para ver onde deu tudo. Se não anotar, pode ir esquecendo ao meio do caminho. Então o objetivo deste passo é para quando o contexto for muito complexo que geraria um gasto absurdo de TOKENS ou mesmo faria a IA se perder legal, para você mesmo passar ele para ela.

## ESCREVER PSEUDOCÓDIGO

Pseudocódigo são scripts feitos em linguagem natural. Não precisa seguir estruturas conhecidas como usar LOOPS, instanciação de classes. Pode ser algo bem simples como:

> SE ISSO → Faça Isso.

A ideia aqui é simplesmente seguir um rumo lógico para seu código.

O pseudocódigo serve para mostrar para a IA seu plano inicial. Assim quando ela gerar o código, você vai ter uma noção da estrutura (que é o mais importante) e não detalhes específicos do código.
