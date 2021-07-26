<p>
	Элемент <LE>applet</LE> служит для вставки специальных прогламм написанных на языке Java. Данный элемент устарел и не поддерживается современными браузерами.
</p>

<p>
	 Взамен необходимо использовать более гибкий тег <LE>object</LE>. Между открывающим и закрывающим тегом можно добавить текст, который будет отображаться в браузере, если он не поддерживает апплеты. В противном случае текст не выводится.
</p>

<ExampleBox>

<Code>
{`
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN"
  "http://www.w3.org/TR/html4/strict.dtd">
<html>
    <head>
    <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
    <title>Тег APPLET</title>
    </head>
    <body>
        <p>Текущее время: <applet code="Clock.class" width="60" height="10">
        Ваш браузер не поддерживает Java-апплеты.
        </applet></p>
    </body>
</html>
`}
</Code>

</ExampleBox>




