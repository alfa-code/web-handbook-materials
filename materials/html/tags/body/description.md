<p>
	Элемент <LE>body</LE> представляет содержимое веб страницы (документ / document). В документе может быть только один элемент <LE>body</LE>
</p>

<p>
	Элемент <LE>body</LE> содержит в себе атрибуты для <LE>Window</LE>. Он также отражает их IDL-атрибуты.
</p>

<p>
	Помощники <LE>Window</LE>, названные Window-reflecting body element event handler set, отражают окно, представленное в элементе <LE>body</LE>, заменяют event handlers теми же именами, которые обычно поддерживаются элементами HTML.
</p>


<ExampleBox>
	На этой странице обновляется индикатор, чтобы показать, находится ли пользователь в сети:

<Code>
{`
<!DOCTYPE HTML>
<html lang="en">
 	<head>
  	<title>В сети или нет?</title>
  	<script>
  		 function update(online) {
    	 document.getElementById('status').textContent =
      	 online ? 'Online' : 'Offline';
   	}
 	</script>
 	</head>
 	<body 	ononline="update(true)"
      		onoffline="update(false)"
       		onload="update(navigator.onLine)">
  			<p>Ты: <span id="status">(Неизвестно)</span></p>
 	</body>
</html>
`}
</Code>

</ExampleBox>




