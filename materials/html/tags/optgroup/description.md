<p>
	 Элемент <LE>optgroup</LE> представляет собой группу элементов <LE>option</LE> с общей меткой.
</p>

<p>
   Группа элементов <LE>option</LE> одного элемента состоит из элементов <LE>option</LE>, которые являются потомками элемента <LE>optgroup</LE>.
</p>

<p>
   При отображении элементов <LE>option</LE> в элементах  <LE>select</LE>, пользовательские агенты должны показывать элементы <LE>option</LE> таких групп как связанные друг с другом и отдельные от других элементы <LE>option</LE>.
</p>

<p>
   Атрибут <LA>disabled</LA> может использоваться для одновременного отключения группы элементов <LE>option</LE>.
</p>

<p>
   Атрибут <LA>label</LA> должен быть указан. Его значение показывает имя группы для пользовательского интерфейса. Пользовательские агенты должны использовать значение этого атрибута при маркировке группы элементов <LE>option</LE> в элементе <LE>select</LE>.
</p>

<p>
   Атрибуты <LA>disabled</LA> и <LA>label</LA> должны отражать соответствующие атрибуты содержимого с тем же именем.
</p>

<ExampleBox>

В следующем фрагменте показано, как можно предложить набор уроков из трех курсов в <LE>select</LE> виджете выбора:

<Code>
{`
<form action="courseselector.dll" method="get">
    <p>Какой кукрс вы бы хотели посмотреть сегодня?
    <p><label>Курсы:
    <select name="c">
    <optgroup label="8.01 Physics I: Classical Mechanics">
        <option value="8.01.1">Лекция 01: Сила десяти
        <option value="8.01.2">Лекция 02: Кинематика
        <option value="8.01.3">Лекция 03: Вектора
    <optgroup label="8.02 Electricity and Magnetism">
        <option value="8.02.1">Лекция 01: Ято держит весь мир вместе?
        <option value="8.02.2">Лекция 02: Электрические поля
        <option value="8.02.3">Лекция 03: Электричество
    <optgroup label="8.03 Physics III: Vibrations and Waves">
       <option value="8.03.1">Лекция 01: Периодичность
       <option value="8.03.2">Лекция 02: Биты
       <option value="8.03.3">Лекция 03: Демпинг
    </select>
    </label>
    <p><input type=submit value="▶ Play">
</form>
`}
</Code>

</ExampleBox>

