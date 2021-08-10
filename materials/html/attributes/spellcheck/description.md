<p>
	Указывает браузеру проверять или нет правописание и грамматику в тексте. Хотя атрибут можно устанавливать практически для всех элементов, результат будет заметен только для полей форм (<LA>input</LA>, <LA>textarea</LA>), а также редактируемых элементов.
</p>

<ExampleBox>

<Code>
{`
<!DOCTYPE html>
<html>
	 <head>
		  <meta charset="utf-8">
		  <title>spellcheck</title>
	 </head>
	 <body>
		  <p contenteditable="true" spellcheck="false">
		   Не лѣпо ли ны бяшетъ, братіе, начяти 
		   старыми словесы трудныхъ повѣстій 
		   о пълку Игоревѣ, Игоря Святъславлича?
		  </p>
	 </body>
</html>
`}
</Code>

</ExampleBox>


