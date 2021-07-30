<p>
	Содержимое тега <LE>noframes</LE> отображается в браузере, когда он не поддерживает фреймы и не умеет их интерпретировать. Браузеры, которые работают с фреймами, полностью игнорируют содержимое тега <LE>noframes</LE>. Как правило, внутри этого тега располагается текст, информирующий пользователя о том, что его браузер фреймы не поддерживает или с предложением перейти на страницу без фреймов.
</p>

<ExampleBox>

<Code>
{`
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Frameset//EN"
  "http://www.w3.org/TR/html4/frameset.dtd">
<html>
	  <head>
		    <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
		    <title>Тег NOFRAMES</title>
	  </head>
	  <frameset cols="100,*">
		    <frame src="menu.html" name="leftFrame">
		    <frame src="content.html" name="mainFrame">
		    <noframes>Ваш браузер не поддерживает фреймы.</noframes>
	  </frameset>
</html>
`}
</Code>

</ExampleBox>






