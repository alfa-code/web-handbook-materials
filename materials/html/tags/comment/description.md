<p>
	Добавляет комментарий в код документа. Тег <LE>comment</LE> допустимо использовать только в <LE>body</LE>.
</p>

<ExampleBox>

<Code>
{`
	<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
	<html>
 	<head>
  	<meta http-equiv="Content-Type" content="text/html; charset=utf-8">
  			<title>Тег COMMENT</title>
  	<style type="text/css">
  			div {
   			background: green; 
   			color: white; 
    		padding: 4px; 
  			}
   			div.ie {
    		background: maroon; 
  			}
  	</style>
 	</head>
 	<body>
  			 <comment><div class="ie">Этот текст не виден в браузере Internet Explorer</div></comment>
   			<div>Этот текст показывается во всех браузерах</div>
 	</body>
	</html>
`}
</Code>

</ExampleBox>




