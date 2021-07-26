<p>
  Элемент <LE>form</LE> представляет собой гиперссылку, которой можно управлять с помощью набора связанных с формой элементов, некоторые из которых могут представлять редактируемые значения, которые могут быть отправлены на сервер для обработки.
</p>

<ExampleBox>

	В этом примере показаны две формы поиска:

<Code>
{`
<form action="https://www.google.com/search" method="get">
 		<label>Google: <input type="search" name="q"></label> <input type="submit" value="Search...">
</form>
<form action="https://www.bing.com/search" method="get">
 		<label>Bing: <input type="search" name="q"></label> <input type="submit" value="Search...">
</form>
`}
</Code>

</ExampleBox>




