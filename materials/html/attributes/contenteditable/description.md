<p>
	Атрибут содержимого <LA>contenteditable</LA> - это перечислимый атрибут, ключевыми словами которого являются пустая строка, true и false. Ключевое слово false соответствует ложному состоянию. Кроме того, существует третье состояние, состояние наследования, которое является отсутствующим значением по умолчанию и недопустимым значением по умолчанию.
</p>

<p>
	true состояние указывает, что элемент доступен для редактирования. Состояние наследования указывает, что элемент доступен для редактирования. Состояние false указывает, что элемент нельзя редактировать.
</p>

<ExampleBox>

Например, рассмотрим страницу, которая имеет форму и текстовое поле для публикации новой статьи, где пользователь, как ожидается, напишет статью, используя HTML:

<Code>
{`
<form method=POST>
	 <fieldset>
		  <legend>Новая статья</legend>
		  <textarea name=article>&lt;p>Hello world.&lt;/p></textarea>
	 </fieldset>
	 <p><button>Опубликовать</button></p>
</form>
`}
</Code>

Когда сценарии включены, элемент <LE>textarea</LE> можно заменить элементом управления форматированным текстом, используя атрибут <LA>contenteditable</LA>:

<Code>
{`
<form method=POST>
	 <fieldset>
		  <legend>Новая статья</legend>
		  <textarea id=textarea name=article>&lt;p>Hello world.&lt;/p></textarea>
		  <div id=div style="white-space: pre-wrap" hidden><p>Привет, мир.</p></div>
		  <script>
			   let textarea = document.getElementById("textarea");
			   let div = document.getElementById("div");
			   textarea.hidden = true;
			   div.hidden = false;
			   div.contentEditable = "true";
			   div.oninput = (e) => {
			   textarea.value = div.innerHTML;
		   };
		  </script>
	 </fieldset>
	 <p><button>Опубликовать</button></p>
</form>
`}
</Code>

</ExampleBox>




