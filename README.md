# RegEx
Aprendendo RegEx - Expressões Regulares
https://regexr.com/

<<<<<<<< Operadores Literais >>>>>>>>>>
\s = space (Espaço em uma casa).

( [Oo][Ll][Aa]\s[Mm][Uu][Nn][Dd][Oo] )

Cada [] quer dizer uma casa e foi pesquisado Mausculo e Minusculo da palavra Olá Mundo.

<<<<<<<< Caracteres de Escape >>>>>>>>>

\d => Digito (Qualquer número de 0 a 9).

(31) 65523-3575

( -\d\d\d5 ) -> Aqui vamos pesquisar onde o ultimo caractere for 5, depois do -.

<<<<<<<< Caracteres de Especiais >>>>>>>>>

Este é um exemplo.

( \. ) -> Para pesquisar um caractere especial é necessario colicar uma \ antes.

<<<<<<<< Meta de Caractere >>>>>>>>>

GWWA

(G..A) -> Para o texto acima usamos essa expresão; ( . ) -> Quer dizer qualquer coisa.

Eu sou eu todo dia.
( ^Eu ) Para pesquisar Eu em todo inicio de paragrafo.
( ^\w ) Para pesquisar qualquer caractere em inicio de paragrafo.
( \.$ ) Para pesquisar o ponto no final da linha; ( $ ) -> Quer dizer o final da linha.

123456

[1-5] -> Para pesquisar um caractere de 1 ao 5; [] -> Quer dizer um conjunto.

<<<<<<<< Codificadores >>>>>>>>>

carro carroceiro capoteiro castro cadastro carra carroceria 

( c\w{3,7}o ) -> Para pesquisar um forma com inicio c e após 3 carractes 'o' no final ou após 7 carractere 'o' no final -> {0,2} -> Quantificar a quantidade do caractere vai está presente.


( c\w{6,} ) - Para quando a gente tem um minimo de caractere que desejamos mas não sabemos o maximo. 


color colour
( colou?r ) - Para quando o caractere pode existir ou quando o caractere pode não existir. Ou seja o u a esquerda do ? fica opcional.

va
voa
vooa
voooa
vooooa
voooooa
( vo*a ) - O * serve para pegar de um caractere e ir até o final a, assim pegando todos acima 
( vo+a ) - O + pega exatamente do vo e o final a.


<p>Primeiro Paragrafo</p>
<p>Segundo Paragrafo</p>
<p>Terceiro Paragrafo</p>
( <p>.*</p> ) -> Vai pegar tudo, do inicio ao final como se fosse uma seleção apenas.
( <p>.*?</p> ) -> vai pegar tudo, separando cada inicio e final como se for um vetor.


<<<<<<<< Operadores Logicos >>>>>>>>>

<p>Primeiro Paragrafo</p>
<p>Segundo Paragrafo</p>
<p>Terceiro Paragrafo</p>
(<p>(Primeiro|Segundo)\sParagrafo</p>) -> | Vai representar operador logico OU.


Este é um teste de expressão 
[^abc] -> ^ dentro do [] vai significar uma negação, ou seja tudo que não tenha abc.
 

Jennifer
Jennifer Teste 
(Jennifer(?\sTeste)) -> Aqui vai pesquisar todas às Jeniffer que após o nome tem 'Teste'.

Jennifer
Jennifer Teste 
(Jennifer(?\sTeste)) -> Aqui vai pesquisar todas às Jeniffer diferente que após o nome tem 'Teste'.

Tudo acima acima sim
(\b(\w+)\s\1\b) -> Aqio vai referenciar grupo anteriores. 

