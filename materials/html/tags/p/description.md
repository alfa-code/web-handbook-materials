<p>
    Элемент <LE>p</LE> представляет собой абзац.
</p>

<ExampleBox>
	Следующие примеры соответствуют фрагментам HTML:

<Code>
{`
<p>Котенок осторожно уселся на кусок
ковровой дорожки.</p>
<fieldset>
	 <legend>Личная информация</legend>
	 <p>
		   <label>Имя: <input name="n"></label>
		   <label><input name="anon" type="checkbox"> Скрыть от других пользователей</label>
	 </p>
	 <p><label>Адрес: <textarea name="a"></textarea></label></p>
</fieldset>
<p>Когда-то был пример, <br>
Разметка сомнительного качества. <br>
Валидатор не работал, <br>
Итак, автору было плохо, <br>
Чтобы из ошибки сделать рифму.</p>
`}
</Code>

</ExampleBox>

<p>
    Элемент <LE>p</LE> не следует использовать, если более уместен какой-либо конкретный элемент.
</p>

<ExampleBox>

Следующий пример технически верен:

<Code>
{`
<section>
	 <!-- ... -->
	 <p>Последнее изменение: 2001-04-23</p>
	 <p>Автор: fred@example.com</p>
</section>
`}
</Code>

Однако было бы лучше разметить как:

<Code>
{`
<section>
	 <!-- ... -->
	 <footer>Последнее изменение: 2001-04-23</footer>
	 <address>Автор: fred@example.com</address>
</section>
`}
</Code>

Или

<Code>
{`
<section>
	 <!-- ... -->
	 <footer>
	  <p>Последнее изменение: 2001-04-23</p>
	  <address>Автор: fred@example.com</address>
 </footer>
</section>
`}
</Code>

</ExampleBox>







