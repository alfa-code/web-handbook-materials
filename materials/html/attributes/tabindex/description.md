<p>
	Атрибут <LA>tabindex</LA> определяет последовательность перехода между ссылками при нажатии на кнопку tab. Любое целое положительное число. Значения выстраиваются последовательно и переход между ссылками происходит от меньшего значения к большему. Значения меньше нуля игнорируются и переход к таким ссылкам не происходит.
</p>

<ExampleBox>

<Code>
{`
<!DOCTYPE HTML>
<html>
	 <head>
		  <meta charset="utf-8">
		  <title>Тег А, атрибут tabindex</title>
	 </head>
	 <body>
		  <table>
			   <tr>
				    <td>
					     <p><a href="1.html" tabindex="1">Ссылка 1</a></p>
					     <p><a href="3.html" tabindex="3">Ссылка 3</a></p>
				    </td>
				    <td>
					     <p><a href="2.html" tabindex="2">Ссылка 2</a></p>
					     <p><a href="4.html" tabindex="4">Ссылка 4</a></p>
				    </td>
			   </tr>
		  </table>
	 </body>
</html>
`}
</Code>

</ExampleBox>


