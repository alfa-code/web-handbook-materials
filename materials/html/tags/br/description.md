<p>
  Элемент <LE>br</LE> представляет собой разрыв строки.
</p>

<p>
  Элементы <LE>br</LE> должен использоваться только для разрывов строк, которые являются частью текста, например, в стихах или адресах.
</p>

<ExampleBox>

Следующий пример - правильное использование элемента <LE>br</LE>

<Code>
{`
<p>
    П. Шермен<br>
    42 Улица<br>
    Сидней
</p>
`}
</Code>

</ExampleBox>

<p>
  Элементы <LE>br</LE> нельзя использовать для разделения тематических групп в абзаце.
</p>

<ExampleBox>

Следующие примеры не соответствуют требованиям, поскольку они злоупотребляют элементом <LE>br</LE>:

<Code>
{`
<p>
    <a ...>34 comments.</a><br>
    <a ...>Add a comment.</a>
</p>
`}
</Code>

<Code>
{`
<p>
    <label>Name: <input name="name"></label><br>
    <label>Address: <input name="address"></label>
</p>
`}
</Code>

Вот правильный вариант:

<Code>
{`
<p>
    <a ...>34 comments.</a>
</p>
<p>
    <a ...>Add a comment.</a>
</p>
`}
</Code>

<Code>
{`
<p>
    <label>Name: <input name="name"></label>
</p>
<p>
    <label>Address: <input name="address"></label>
</p>
`}
</Code>

</ExampleBox>

<p>
  Если абзац состоит только из одного элемента <LE>br</LE>, он представляет собой пустую строку (например, как в шаблоне). Такие пустые строки нельзя использовать в презентационных целях.
</p>

<p>
  Любое содержимое внутри элементов <LE>br</LE> не должно считаться частью текста вокруг.
</p>