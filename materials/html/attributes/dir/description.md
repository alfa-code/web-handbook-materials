<p>
	Задает направление и отображение текста — слева направо или справа налево. Браузеры обычно самостоятельно различают направление текста, если он задан в кодировке Юникод, но с помощью атрибута <LA>dir</LA> можно указать, в каком направлении отображать текст. Для арабских и еврейских символов приоритетным является направление, заложенное в Юникод, поэтому на них атрибут <LA>dir</LA> действовать не будет.
</p>

<ExampleBox>

<Code>
{`
<!DOCTYPE html>
<html>
	 <head>
		  <meta charset="utf-8">
		  <title>Атрибут dir</title>
	 </head>
	 <body>
		  <p dir="rtl">שבת — суббота</p>
		  <p>В ашкеназском произношении звучит как «ша́бос» (идиш «ша́бес»), 
		   а в сефардском — как «шаба́т».</p>
	 </body>
</html>
`}
</Code>

</ExampleBox>



