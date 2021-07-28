<p>
 	Элемент <LE>label</LE> представляет заголовок в пользовательском интерфейсе. Заголовок может быть связан с конкретным элементом управления формы, известным как элемент <LE>label</LE>, либо с помощью атрибута <LA>for</LA>, либо путем помещения элемента управления формы внутри самого элемента <LE>label</LE>.
</p>

<ExampleBox>

В следующем примере показаны три элемента управления формой, каждый с <LE>label</LE>, два из которых имеют небольшой текст, показывающий правильный формат для использования.

<Code>
{`
<p><label>Полное имя: <input name=fn> <small>Формат: Фамилия Имя</small></label></p>
<p><label>Возраст: <input name=age type=number min=0></label></p>
<p><label>Код: <input name=pc> <small>Формат: AB12 3CD</small></label></p>
`}
</Code>

</ExampleBox>

<ExampleBox>

В этом (несоответствующем) примере показано, что происходит с <LE>NodeList</LE> и какие <LE>label</LE> возвращаются при изменении атрибута <LA>type</LA> элемента <LA>input</LA>.

<Code>
{`
<!doctype html>
<p><label><input></label></p>
<script>
	 	const input = document.querySelector('input');
	 	const labels = input.labels;
	 	console.assert(labels.length === 1);

	 	input.type = 'hidden';
	 	console.assert(labels.length === 0); //  input не контролируется больше label
	 	console.assert(input.labels === null);

	 	input.type = 'checkbox';
	 	console.assert(labels.length === 1); // input снова под label контролем
	 	console.assert(input.labels === labels); // то же значение, что было изначально
</script>
`}
</Code>

</ExampleBox>







