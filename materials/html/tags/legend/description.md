<p>
	Элемент <LE>legend</LE> представляет собой заголовок для остального содержимого родительского элемента <LE>fieldset</LE> элемента <LE>legend</LE>, если таковой имеется.
</p>

<p>
	Поведение атрибута IDL <LA>form</LA> зависит от того, находится ли элемент <LE>legend</LE> в элементе <LE>fieldset</LE>  или нет. Если <LE>legend</LE> имеет элемент <LE>fieldset</LE> в качестве своего родительского элемента, тогда атрибут IDL <LA>form</LA> должен возвращать то же значение, что и атрибут IDL <LA>form</LA> для элемента <LE>fieldset</LE>. В противном случае он должен вернуть  свое исходное значение.
</p>







