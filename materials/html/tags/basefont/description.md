<p>
	Тег <LE>basefont</LE> предназначен для задания шрифта, размера и цвета текста по умолчанию. Указанные значения будут использоваться во всем документе за исключением тега <LE>font</LE>, в котором можно переопределить параметры оформления текста. Допускается использование тега в контейнере <LE>head</LE> или <LE>body</LE>, причем несколько раз. Это позволяет изменять вид шрифта для части документа.
</p>

<ExampleBox>

<Code>
{`
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN"
  "http://www.w3.org/TR/html4/loose.dtd">
<html>
 	<head>
  	<meta http-equiv="Content-Type" content="text/html; charset=utf-8">
 			 <title>Тег BASEFONT</title>
 	</head>
 	<body>
  			<basefont face="Arial, Helvetica, sans-serif" size="4" color="maroon">
  			<p>Страница оформлена с помощью тега BASEFONT</p>
 	</body>
`}
</Code>

</ExampleBox>




