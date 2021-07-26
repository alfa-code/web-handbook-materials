<p>
	Элемент <LE>acronym</LE> служит для выделения в тексте акронима. Данный элемент устарел, используйте элемент <LE>abbr</LE>
</p>

<p>
	 В отличие от аббревиатуры, акроним — это устоявшееся сокращение, которое применяется как самостоятельное слово. 
</p>

<p>
	По умолчанию, текст заключенный в контейнере <LE>acronym</LE> подчеркивается пунктирной линией.
</p>

<ExampleBox>

<Code>
{`
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN"
  "http://www.w3.org/TR/html4/strict.dtd">
 	<html>
  	<head>
   	<meta http-equiv="Content-Type" content="text/html; charset=utf-8">
   		<title>Тег ACRONYM</title>
   	<style type="text/css">
    acronym {
     border-bottom: 1px dashed blue; 
     color: maroon; 
    }
   	</style>
  	</head>
  	<body> 
  		<p>Северную Америку многие воспринимают толкьо как <acronym title="Название страны">США</acronym>.</p>
 	</body> 
	</html>
`}
</Code>

</ExampleBox>




