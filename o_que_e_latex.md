## O que é LaTex

Colocado de forma bem simples, LaTeX é uma sistema de edição de texto que separa o conteúdo da forma.
Conteúdo é o texto propriamente dito, a história que você está contando; e forma é a aparência desse
texto, como por exemplo, se a palavra está em negrito, se o fonte da letra é maior ou menor, etc.

Vamos a um exemplo. Se você tem alguma familiaridade com editores de texto tradicionais, tais como o
Microsoft Word, você edita um texto mais ou menos assim: você escreve o conteúdo ("O cachorro latiu.")
e resolve colocar a palavra "cachorro" em negrito. Para isso, você marca a palavra "cachorro" com o mouse
e busca na barra de ferramentas do software Word o ícone que converte para negrito. Clica nesse ícone
e a palavra "cachorro" aparece em negrito na tela do seu computador, instantaneamente.

Para obter tal efeito usando LaTeX o procedimento é composto por duas etapas. Na primeira etapa
você escreve o seu texto (como faria no Word) e indica qual palavra deve aparecer em negrito
(veremos como fazer isso logo adiante). Na segunda etapa você usa um progrma para converter o que 
você escreveu em um documento que mostre as alterações na tela do computador (e que você possa
imprimir também).

Primeira etapa. Você abre um software qualquer
que possa ser usado para se escrever um texto sem formatação alguma (por exemplo, o Bloco de Notas do Windows).
Você escreve o conteúdo do seu texto: "o cachorro latiu". Para fazer a palavra cachorro aparecer em
negrito, você coloca alguns comandos no corpo do texto para indicar que ela deve ficar em negrito.
Esse comando é o seguinte: 

    \textbf{}
    
A barra invertida indica que teremos um comando a seguir.
textbf é o comando que indica que o text deve ser bold face.
As chaves marcam o início e o fim do texto a ser colocado em negrito (bold face).
É mais complicado do que o Word, mas o resultado será equivalente.


    O \textbf{cachorro} latiu.
    
Um último detalhe necessário antes de passarmos para a etapa dois: a primeira linha do arquivo
onde está seu texto precisar ter um comando geral para dizer que esse é um arquivo em LaTeX
e passar alguns detalhes de como o documento final será formatado. O comando é o seguinte:

    \documentclass{article}

Então, seu arquivo completo fica assim:

    \documentclass{article}

    O \textbf{cachorro} latiu.

Uma vez feito isso nada acontece! Você continua a ver esses comandos misturados com seu texto na tela do 
seu computador dentro do programa Bloco de Notas. Precisamos da etapa dois.

Etapa dois. Você salva esse arquivo do Bloco de Notas e roda um segundo programa, um 
processador LaTeX, que vai converter todos os comandos do texto em uma tipografia correspondente
(no caso, colocar a palavra cachorro em negrito). O resultado de se rodar esse segundo programa é
um arquivo PDF, que você pode ler na tela do computador ou imprimir.

É assim que o LaTeX funciona, numa explicação bastante simplificada.

A pergunta do milhão é: para que essa complicação toda? Não é muito mais fácil usar o Microsoft Word
(ou software equivalente)?

