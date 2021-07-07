<p>
	Элемент <LE>fieldset</LE> представляет собой набор элементов управления формой (или другого содержимого), сгруппированных вместе, необязательно с заголовком. Заголовок задается первым элементом <LE>legend</LE>, который является дочерним элементом элемента <LE>fieldset</LE>, если таковой имеется. Остальные дочерние элементы образуют группу.
</p>

<p>
	Атрибут <LA>disabled</LA>, если он указан, вызывает отключение всех дочерних элементов <LE>fieldset</LE>, за исключением тех, которые являются дочерними элементами первого элемента <LE>legend</LE> элемента <LE>fieldset</LE>, если таковые имеются. 
</p>

<p>
	Элемент <LE>fieldset</LE> является неактивным набором полей, если он соответствует любому из следующих условий:
</p>

<p>
    <ul>
        <li>Указывается <LA>disabled</LA> атрибут</li>
        <li>Это дочерний элемент другого элемента <LE>fieldset</LE>, для которого указан атрибут <LA>disabled</LA>, и не является дочерним элементом <LE>legend</LE> и <LE>fieldset</LE>, если таковой имеется.</li>
    </ul>
</p>

<p>
	Атрибут <LA>form</LA> используется для явного связывания элемента <LE>fieldset</LE> с его главным элементом. Атрибут <LA>name</LA> представляет имя элемента.
</p>

<p>
	Атрибут <LA>disabled</LA> IDL должен отражать атрибут содержимого с тем же именем.
</p>

<p>
	Атрибут IDL <LA>type</LA> должен возвращать строку «fieldset».
</p>

<p>
	Атрибут IDL <LE>elements</LE> должен возвращать HTMLCollection в корень элемента <LE>fieldset</LE>.
</p>

<p>
	Атрибуты <LA>willValidate</LA>, <LA>validity</LA> и <LA>validationMessage</LA>, а также методы checkValidity (), reportValidity () и setCustomValidity () являются частью API проверки. Атрибуты IDL <LA>name</LA> и <LA>form</LA> являются частью API форм элемента.
</p>

<ExampleBox>

В этом примере показан элемент <LE>fieldset</LE>, используемый для группировки набора связанных элементов управления:

<Code>
{`
<fieldset>
 	<legend>Экран</legend>
 	<p><label><input type=radio name=c value=0 checked> Черно-белое</label>
 	<p><label><input type=radio name=c value=1>Белое на черном</label>
 	<p><label><input type=checkbox name=g> Использовать серый</label>
 	<p><label>Контраст<input type=range name=e list=contrast min=0 max=100 value=0 step=1></label>
 	<datalist id=contrast>
  		<option label=Normal value=0>
  		<option label=Maximum value=100>
	</datalist>
</fieldset>
`}
</Code>

</ExampleBox>

<ExampleBox>

В следующем фрагменте показан <LE>fieldset</LE> с отметкой в <LE>legend</LE>, который определяет, включен ли <LE>fieldset</LE>. Содержимое <LE>fieldset</LE> состоит из двух обязательных текстовых элементов управления и дополнительного элемента управления годом / месяцем.

<Code>
{`
<fieldset name="clubfields" disabled>
 	<legend> <label>
 	 <input type=checkbox name=club onchange="form.clubfields.disabled = !checked">
 		 Используйте клубную карту
 	</label> </legend>
 	<p><label>Название карты: <input name=clubname required></label></p>
	<p><label>Номер карты: <input name=clubnum required pattern="[-0-9]+"></label></p>
 	<p><label>Дата: <input name=clubexp type=month></label></p>
</fieldset>
`}
</Code>

</ExampleBox>

<ExampleBox>

Вы также можете вкладывать элементы в <LE>fieldset</LE>. Вот пример, расширяющий предыдущий, показывающий это:

<Code>
{`
<fieldset name="clubfields" disabled>
	<legend> <label>
  	<input type=checkbox name=club onchange="form.clubfields.disabled = !checked">
  		Использовать клубную карту
 	</label> </legend>
 	<p><label>Название карты: <input name=clubname required></label></p>
<fieldset name="numfields">
  	<legend> <label>
   	<input type=radio checked name=clubtype onchange="form.numfields.disabled = !checked">
  		 На моей карте есть номер
  	</label> </legend>
  	<p><label>Номер карты: <input name=clubnum required pattern="[-0-9]+"></label></p>
</fieldset>
<fieldset name="letfields" disabled>
 	<legend> <label>
	<input type=radio name=clubtype onchange="form.letfields.disabled = !checked">
	   На моей карте есть буквы
  	</label> </legend>
 	 <p><label>Код: <input name=clublet required pattern="[A-Za-z]+"></label></p>
</fieldset>
</fieldset>
`}
</Code>

</ExampleBox>

<ExampleBox>

В этом примере показано группирование элементов управления, в котором элемент <LE>legend</LE> обозначает группировку, а вложенный элемент заголовка отображает группировку в структуре документа:

<Code>
{`
<fieldset>
 	<legend> <h2>
  		Как вы можете связаться с нами?
 	</h2> </legend>
 	<p> <label>
 	<input type=radio checked name=contact_pref>
 		 Телефон
 	</label> </p>
 	<p> <label>
 	 <input type=radio name=contact_pref>
 		 Текст
	</label> </p>
 	<p> <label>
 	 <input type=radio name=contact_pref>
 		 Почта
 	</label> </p>
</fieldset>
`}
</Code>

</ExampleBox>




