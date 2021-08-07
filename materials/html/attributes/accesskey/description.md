<p>
	Для всех элементов HTML может быть установлен атрибут <LA>accesskey</LA>. Значение атрибута <LA>accesskey</LA> используется пользовательским агентом в качестве руководства для создания сочетания клавиш, которое активирует или фокусирует элемент.
</p>

<p>
	Значение должно быть упорядоченным набором, разделенным пробелами, ни один из которых не идентичен другому, и каждый из которых должен иметь ровно одну кодовую точку.
</p>

<ExampleBox>

В следующем примере представлены различные ссылки с клавишами доступа, чтобы пользователи клавиатуры, знакомые с сайтом, могли быстрее переходить на соответствующие страницы:

<Code>
{`
<nav>
	 <p>
		  <a title="Активность" accesskey="A" href="/Consortium/activities">Активность</a> |
		  <a title="Рекомендации" accesskey="T" href="/TR/">Рекомендации</a> |
		  <a title="Алфавит" accesskey="S" href="/Consortium/siteindex">Алфавит</a> |
		  <a title="О сайте" accesskey="B" href="/Consortium/">О сайте</a> |
		  <a title="Контакты" accesskey="C" href="/Consortium/contact">Контакты</a>
	 </p>
</nav>
`}
</Code>

В следующем примере в поле поиска даются два возможных ключа доступа: «s» и «0» (в указанном порядке). Пользовательский агент на устройстве с клавиатурой может выбрать Ctrl + Alt + S в качестве сочетания клавиш, в то время как пользовательский агент на небольшом устройстве с простой цифровой клавиатурой может выбрать только простую неукрашенную клавишу 0:

<Code>
{`
<form action="/search">
	 <label>Search: <input type="search" name="q" accesskey="s 0"></label>
	 <input type="submit">
</form>
`}
</Code>

В следующем примере для кнопки описаны возможные ключи доступа. 

<Code>
{`
<input type=submit accesskey="N @ 1" value="Compose">
...
<script>
 	function labelButton(button) {
   		if (button.accessKeyLabel)
    	button.value += ' (' + button.accessKeyLabel + ')';
 }
 	var inputs = document.getElementsByTagName('input');
 		for (var i = 0; i < inputs.length; i += 1) {
  		if (inputs[i].type == "submit")
     	labelButton(inputs[i]);
 }
</script>
`}
</Code>

</ExampleBox>




