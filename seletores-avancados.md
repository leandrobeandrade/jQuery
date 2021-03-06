### $( "attribute" ) - Seleciona elementos que possuam a propriedade especificada com valor específico.

	$( "input" ).prop("required", true)  // seleciona inputs e define a propriedade required como true
	
### $( ":element" ) - Seleciona todos os elementos de todos os tipos.

	$( "div:button" ).comandos  //  seleciona todos os botões dentro da div
	
### $( ":not()" ) - Seleciona elementos não encontrados nos parâmetros passados.
	
	$( "input:not(:checked)" ).comandos  //  seleciona inputs com o atributo checked falso
	
### $( ":lang()" ) - Seleciona determinada linguagem no html.

	$( "div:lang(pt-br)" ).comandos  //  seleciona a div com o atributo lang pt-br

### $( ":disabled" ) - Seleciona elementos com o atributo disabled.

	$( "input:disabled" ).comandos  //  seleciona inputs desabilitado
	
### $( ":empty" ) - Seleciona elementos vazios.
	
	$( "p:empty" ).comandos  //  seleciona p vazios
	
### $( ":visible" ) - Seleciona elementos que não estão com display none.

	$( "div:visible" ).comandos  //  seleciona divs visíveis no html
	
### $( ":hidden" ) - Seleciona elementos que estão com display none.

	$( "div:hidden" ).show("fast");  //  mostra divs que não estão aparecendo no html  
	
### $( ":contains(texto)" ) - Seleciona todos os elementos que possuem um determinado texto passado no parâmetro.

	$( "p:contains('Teste')" ).comandos  //  seleciona tags p que contem a palavra Teste
	
### $( ":eq(index)" ) - Seleciona o index dos elementos referenciados. 

	$( "li:eq(2)" ).comandos  //  seleciona a terceira li em uma ul
	
### $( ":odd" ) - Seleciona elementos ímpares.

	$( "tr:odd" ).comandos  // seleciona linhas ímpares em uma tabela
	
### $( ":even" ) - Seleciona elementos pares.

	$( "tr:even" ).comandos //  seleciona linhas pares em uma tabela
	
### $( ":first" ) - Seleciona o primeiro elemento de um conjunto de elementos.

	$( "p:first" ).comandos //  seleciona o primeiro p
	
### $( ":last" ) - Seleciona o último elemento de um conjunto de elementos.

	$( "p:last" ).comandos  //  seleciona o último p
	
### $( ":last-child" ) - Seleciona o último filho em um nó Html.

	$( "div span:last-child" ).comandos  //  seleciona o último span dentro de uma div

### $( ":only-child" ) - Seleciona todos os elementos que são filhos únicos de seus pais.

	$( "div span:only-child" ).comandos // seleciona apenas o span dentro de div que só tem este span
	
### $( ":only-of-type" ) - Seleciona todos os elementos que não têm irmãos com o mesma tag.

	$( "div span:only-of-type" ).comandos // seleciona apenas spans se não houver outros span na div
	
### $( ":gt(index)" ) - Seleciona elementos com o index maior em um conjunto de elementos.

	$( "td:gt(4)" ).comandos // seleciona células depois da quinta célula em uma tabela
	
### $( ":lt(index)" ) - Seleciona elementos com o index menor em um conjunto de elementos.

	$( "td:lt(4)" ).comandos  //  seleciona células antes da quarta célula em uma tabela
	
### $( ":nth-child(index)" ) - Seleciona elementos a partir de determinada localização.

	$( "ul li:nth-child(2)" ).comandos  //  seleciona o segundo li em uma ul
	
### $( ":nth-last-child(index)" ) - Seleciona elementos a partir de determinada localização do último para o primeiro.

	$( "ul li:nth-last-child(2)" ).comandos  //  seleciona o segundo li de baixo para cima em uma ul
	
### $( ":nth-of-type(index)" ) - Seleciona elementos do mesmo tipo em determinada localização.

	$( "span:nth-of-type(2)" ).comandos;  //  seleciona o segundo span 
	
### $( ":nth-last-of-type(index)" ) - Seleciona elementos do mesmo tipo a partir de determinada localização do último para o primeiro.

	$("span:nth-last-of-type(2)").comandos;  //  seleciona o segundo span de baixo para cima em uma ul	
	
### ( "option:selected" ) - Seleciona itens selecionados em um select.

	$( "select option:selected" ).comados  //  seleciona um ou mais elementos selecionados dentro do select
	
### $( "[atribute=type]" ) - Seleciona qualquer tipo de input.
	
	$( "[input=checkbox]" ).comandos  // seleciona inputs do tipo checkbox
	
### $( "input[atribute='value']" ) - Seleciona com o atributo que tenha o valor especificado.

	$( "input[name='meuInput']" ).comandos  // seleciona o input com o atributo name igual meuInput.
 	
### $( "[attribute|='value']" ) - Seleciona elementos que possuam o atributo especificado com um valor igual a uma string determinada ou que começa com essa seqüência seguida de um hífen (-)

	$( "input[name|='en']" ).comandos  // seleciona en, en-UK


### $( "[attribute*='value']" ) - Seleciona os elementos que possuam o atributo especificado com um valor que contém uma subtring.Exemplo:
			
	$( "input[name*='en']" ).comandos  // seleciona english, en-UK, en


### $( "[attribute^='value']" ) - Seleciona elementos que possuam o atributo especificado com um valor que começa exatamente com uma determinada string.

	$( "input[name^='en']" ).comandos  // seleciona en, english


### $( "[attribute~='value']" ) - Seleciona elementos que possuam o atributo especificado com um valor contendo uma determinada palavra, delimitada por espaços.

	$( "input[name~='en']" ).comandos  // seleciona en glish


### $( "[attribute$='value']" ) - Seleciona elementos que possuam o atributo especificado com um valor que termina exatamente com uma determinada string.A comparação é case sensitive.

	$( "input[name$='en']" ).comandos  // seleciona oficen, milkmen


### $( "[attribute='value']" ) - Seleciona elementos que possuam o atributo especificado com um valor exatamente igual a um determinado valor.

	$( "input[value='en']" ).comandos  // seleciona en


### $( "[attribute!='value']" ) - Selecione elementos que não possuam o atributo especificado ou que tenham o atributo especificado, mas não com um determinado valor.

	$( "input[name!='en']" ).comandos  // seleciona outros


### $( "[attributeFilter1][attributeFilter2][attributeFilterN]" ) - Combina elementos que combinam todos os filtros de atributos especificados.

	$( "input[class][name$='en']" ).comandos  // seleciona classes com name que terminam com en
	
