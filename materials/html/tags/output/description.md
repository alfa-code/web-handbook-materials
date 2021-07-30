<p>
    Элемент <LE>output</LE> представляет собой результат вычислений, выполненных приложением, или результат действия пользователя.
</p>

<ExampleBox>
	Простой калькулятор может использовать выходные данные для отображения расчетных результатов:

<Code>
{`
<form onsubmit="return false" oninput="o.value = a.valueAsNumber + b.valueAsNumber">
	 <input id=a type=number step=any> +
	 <input id=b type=number step=any> =
	 <output id=o for="a b"></output>
</form>
`}
</Code>

В этом примере выходной элемент используется для сообщения результатов вычислений, выполненных удаленным сервером, по мере их поступления:

<Code>
{`
<output id="result"></output>
<script>
	 var primeSource = new WebSocket('ws://primes.example.net/');
	 primeSource.onmessage = function (event) {
	 document.getElementById('result').value = event.data;
 }
</script>
`}
</Code>

</ExampleBox>











