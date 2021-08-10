<p>
	Текст документа может быть набран как на одном языке, так и содержать вставки на других языках, которые могут различаться по своим правилам оформления текста. Например, для русского, немецкого и английского языка характерны разные кавычки, в которые берется цитата. Чтобы указать язык, на котором написан текст внутри текущего элемента и применяется атрибут <LA>lang</LA>. Браузер использует его значение для правильного отображения некоторых символов.
</p>

<ExampleBox>

<Code>
{`
<!DOCTYPE html>
<html>
	 <head>
		  <meta charset="utf-8">
		  <title>Атрибут lang</title>
	  <style>
		   p {
		    font-size: 130%; 
		   }
		   q:lang(de) {
		    quotes: "\201E" "\201C"; 
		   }
		   q:lang(en) {
		    quotes: "\201C" "\201D"; 
		   }
		   q:lang(fr), q:lang(ru) { 
		    quotes: "\00AB" "\00BB"; 
		   }
	  </style>
	 </head>
	 <body>
		  <p>Цитата на французском языке: <q lang="fr">Ce que femme veut, Dieu le veut</q>.</p>
		  <p>Цитата на немецком: <q lang="de">Der Mensch, versuche die Gotter nicht</q>.</p>
		  <p>Цитата на английском: <q lang="en">То be or not to be</q>.</p>
	 </body>
</html>
`}
</Code>

</ExampleBox>


