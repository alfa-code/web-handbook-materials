<p>
	Элемент <LE>noscript</LE> ничего не представляет, если сценарии включены, и представляет своих дочерних элементов, если сценарии отключены. Он используется для представления различной разметки пользовательским агентам, поддерживающим сценарии, и тем, которые не поддерживают создание сценариев, влияя на то, как анализируется документ.

<p>
	Элемент <LE>noscript</LE> нельзя использовать в XML-документах.
</p>

<p>
	Других требований к элементу <LE>noscript</LE> нет. В частности, дочерние элементы элемента <LE>noscript</LE> не освобождаются от отправки формы, создания сценариев и т.д., Даже если для элемента разрешено создание сценариев.
</p>

<ExampleBox>

В следующем примере элемент <LE>noscript</LE> используется для резервирования сценария.

<Code>
{`
<form action="calcSquare.php">
	 <p>Номер</label>:
		  <input id="x" name="x" type="number">
	 </p>
	 <script>
		  var x = document.getElementById('x');
		  var output = document.createElement('p');
		  output.textContent = 'Введите число; оно будет возведено в квадрат сразу!';
		  x.form.appendChild(output);
		  x.form.onsubmit = function () { return false; }
		  x.oninput = function () {
			    var v = x.valueAsNumber;
			    output.textContent = v + ' squared is ' + v * v;
		  };
	 </script>
	 <noscript>
	     <input type=submit value="Calculate Square">
	 </noscript>
</form>
`}
</Code>

Нижеупомянутый метод также полезен в XML-документах, поскольку там запрещен скрипт.

<Code>
{`
<form action="calcSquare.php">
	 <p>
		  <label for=x>Номер</label>:
		  <input id="x" name="x" type="number">
	 </p>
	 <input id="submit" type=submit value="Calculate Square">
	 <script>
		  var x = document.getElementById('x');
		  var output = document.createElement('p');
		  output.textContent = 'Введите число; оно будет возведено в квадрат сразу!';
		  x.form.appendChild(output);
		  x.form.onsubmit = function () { return false; }
		  x.oninput = function () {
		    var v = x.valueAsNumber;
		    output.textContent = v + ' squared is ' + v * v;
		  };
		  var submit = document.getElementById('submit');
		  submit.parentNode.removeChild(submit);
	 </script>
</form>
`}
</Code>

</ExampleBox>






