<p>
	Элемент <LE>head</LE> представляет собой набор метаданных для <LE>Document</LE>.
</p>


<ExampleBox>

Набор метаданных в элементе <LE>head</LE> может быть большим или маленьким. Вот пример очень короткого:

<Code>
{`
<!doctype html>
	<html lang=en>
 		<head>
  			<title>Небольшой документ</title>
 		</head>
 		<body>
 ...
`}
</Code>

Ниже более длинный пример:

<Code>
{`
<!DOCTYPE HTML>
	<HTML LANG="EN">
 		<HEAD>
  			<META CHARSET="UTF-8">
  			<BASE HREF="https://www.example.com/">
  			<TITLE>Пример более длинного документа</TITLE>
  			<LINK REL="STYLESHEET" HREF="default.css">
  			<LINK REL="STYLESHEET ALTERNATE" HREF="big.css" TITLE="Big Text">
  			<SCRIPT SRC="support.js"></SCRIPT>
  			<META NAME="APPLICATION-NAME" CONTENT="Long headed application">
 		</HEAD>
 		<BODY>
 ...
`}
</Code>

</ExampleBox>




