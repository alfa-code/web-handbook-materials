<p>
Элемент <LE>datalist</LE> представляет собой набор элементов <LE>option</LE>, которые предопределяют опции для других элементов ввода (<LE>input</LE>). При рендеринге элемент datalist никак не отображается. Так же не отображаются все дочерние элементы.
</p>

<p>
Список, создаваемый тегом <datalist>, связывается с текстовым полем посредством атрибута id. Его значение должно совпадать со значением атрибута list элемента <LE>input</LE>.

Связка списка опций и элемента ввода осуществляется следующим способом. Элементу ввода (<LE>input</LE>) устанавливается атрибут <LA>list</LA> со значением атрибута <LA>id</LA> элемента <LE>datalist</LE>. Таким образом браузер понимает к кокому элементу ввода привязан тот или иной список опций.
</p>

<ExampleBox>
Простой пример связки элемента ввода и списка опций.
<Code>
{`
<input name=country list="countries">
<datalist id="countries>">
    <option value="Россия">
    <option value="Китай">
</datalist>
`}
</Code>
</ExampleBox>

<ExampleBox>
Еще один пример:
<Code>
{`
<input name=animal list=animals>
<datalist id=animals>
    <option value="Cat">
    <option value="Dog">
</datalist>
`}
</Code>
</ExampleBox>
