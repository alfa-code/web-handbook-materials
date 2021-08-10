<p>
	Атрибут <LA>itemref</LA> предоставляет список идентификаторов элементов, которые содержат дополнительные свойства в других местах документа. Атрибут <LA>itemref</LA> может быть указан только для элементов, которые содержат атрибут <LA>itemscope</LA>. Свойства, которые не являются потомками элемента с атрибутом <LA>itemscope</LA>, можно связать с элементом используя атрибут <LA>itemref</LA>.
</p>

<p>
	Атрибут <LA>itemref</LA> относится к глобальным атрибутам, и может быть использован с любым элементом HTML. Атрибут <LA>itemref</LA> относится к спецификации HTML Microdata.
</p>

<ExampleBox>

<Code>
{`
<div itemscope id="amanda" itemref="a b"></div>
<p id="a">Название: <span itemprop="name">Аманда</span> </p>
<div id="b" itemprop="band" itemscope itemref="c"></div>
<div id="c">
    <p>Группа: <span itemprop="name">Джаз-группа</span> </p>
    <p>Состав: <span itemprop="size">12</span> участников</p>
</div>
`}
</Code>

</ExampleBox>


