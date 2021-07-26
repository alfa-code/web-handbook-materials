<p>
 Тег <LE>frame</LE> определяет свойства отдельного фрейма, на которые делится окно браузера. Этот элемент должен располагаться в контейнере <LE>frameset</LE>, который к тому же задает способ разметки страницы на отдельные области. В каждую из таких областей загружается самостоятельная веб-страница определяемая с помощью атрибута src. Хотя обязательных атрибутов у тега <LE>frame</LE> и нет, рекомендуется задавать каждому фрейму его имя через атрибут <LA>name</LA>. Это особенно важно, если требуется по ссылке из одного фрейма загружать документ в другой.
</p>

<ExampleBox>

<Code>
{`
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Frameset//EN" 
  "http://www.w3.org/TR/html4/frameset.dtd">
<html>
 		<head>
 		<meta http-equiv="Content-Type" content="text/html; charset=utf-8">
  				<title>Тег FRAME</title>
 		</head>
		<frameset rows="80,*" cols="*">
   		<frame src="top.html" name="topFrame" scrolling="no" noresize>
   				<frameset cols="80,*">
     			<frame src="left.html" name="leftFrame" scrolling="no" noresize>
     			<frame src="main.html" name="mainFrame">
   				</frameset>
 		</frameset>

</html>
`}
</Code>

</ExampleBox>




