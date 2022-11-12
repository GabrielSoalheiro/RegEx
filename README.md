# RegEx
Aprendendo RegEx - Expressões Regulares<br/>
https://regexr.com/

<<<<<<<< Operadores Literais >>>>>>>>>><br/>
\s = space (Espaço em uma casa).

( [Oo][Ll][Aa]\s[Mm][Uu][Nn][Dd][Oo] )

Cada [] quer dizer uma casa e foi pesquisado Mausculo e Minusculo da palavra Olá Mundo.

<<<<<<<< Caracteres de Escape >>>>>>>>>

\d => Digito (Qualquer número de 0 a 9).<br/>

(31) 65523-3575<br/> 
( -\d\d\d5 ) -> Aqui vamos pesquisar onde o ultimo caractere for 5, depois do -.

<<<<<<<< Caracteres de Especiais >>>>>>>>>

Este é um exemplo.<br/> 
( \. ) -> Para pesquisar um caractere especial é necessario colicar uma \ antes.

<<<<<<<< Meta de Caractere >>>>>>>>>

GWWA<br/> 
(G..A) -> Para o texto acima usamos essa expresão; ( . ) -> Quer dizer qualquer coisa.

Eu sou eu todo dia.<br/> 
( ^Eu ) Para pesquisar Eu em todo inicio de paragrafo.<br/> 
( ^\w ) Para pesquisar qualquer caractere em inicio de paragrafo.<br/> 
( \.$ ) Para pesquisar o ponto no final da linha; ( $ ) -> Quer dizer o final da linha.

123456<br/> 
[1-5] -> Para pesquisar um caractere de 1 ao 5; [] -> Quer dizer um conjunto.

<<<<<<<< Codificadores >>>>>>>>>

carro carroceiro capoteiro castro cadastro carra carroceria<br/> 
( c\w{3,7}o ) -> Para pesquisar um forma com inicio c e após 3 carractes 'o' no final ou após 7 carractere 'o' no final -> {0,2} -> Quantificar a quantidade do caractere vai está presente.<br/> 
( c\w{6,} ) - Para quando a gente tem um minimo de caractere que desejamos mas não sabemos o maximo. 


color colour<br/> 
( colou?r ) - Para quando o caractere pode existir ou quando o caractere pode não existir. Ou seja o u a esquerda do ? fica opcional.

va<br/> 
voa<br/> 
vooa<br/> 
voooa<br/> 
vooooa<br/> 
voooooa<br/> 
( vo*a ) - O * serve para pegar de um caractere e ir até o final a, assim pegando todos acima <br/> 
( vo+a ) - O + pega exatamente do vo e o final a.<br/> 


< p >Primeiro Paragrafo< /p ><br/> 
< p >Segundo Paragrafo< /p ><br/> 
< p >Terceiro Paragrafo</ p ><br/> 
( < p >.*< /p > ) -> Vai pegar tudo, do inicio ao final como se fosse uma seleção apenas.<br/> 
( < p >.*?</ p > ) -> vai pegar tudo, separando cada inicio e final como se for um vetor.<br/> 


<<<<<<<< Operadores Logicos >>>>>>>>>

< p >Primeiro Paragrafo< /p > <br/> 
< p >Segundo Paragrafo< /p > <br/> 
< p >Terceiro Paragrafo< /p > <br/> 
(< p >(Primeiro|Segundo)\sParagrafo< /p >) -> | Vai representar operador logico OU.<br/> 


Este é um teste de expressão <br/> 
[^abc] -> ^ dentro do [] vai significar uma negação, ou seja tudo que não tenha abc.<br/> 
 

Jennifer<br/> 
Jennifer Teste <br/> 
(Jennifer(?\sTeste)) -> Aqui vai pesquisar todas às Jeniffer que após o nome tem 'Teste'.<br/> 

Jennifer<br/> 
Jennifer Teste <br/> 
(Jennifer(?\sTeste)) -> Aqui vai pesquisar todas às Jeniffer diferente que após o nome tem 'Teste'.<br/> 

Tudo acima acima sim<br/> 
(\b(\w+)\s\1\b) -> Aqui vai referenciar grupo anteriores. <br/> 

