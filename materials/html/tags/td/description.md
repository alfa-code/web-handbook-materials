<p>
	Элемент <LE>td</LE> представляет собой ячейку данных в таблице.
</p>

<p>
	Элемент <LE>td</LE> и его атрибуты <LA>colspan</LA>, <LA>rowspan</LA> и <LA>headers</LA> принимают участие в создании таблицы.
</p>

<p>
	Пользовательские агенты, особенно в невизуальных средах или, где отображение таблицы в виде 2D-сетки нецелесообразно, могут предоставлять пользовательский контекст для ячейки при визуализации содержимого ячейки; например, указание его позиции в модели таблицы или перечисление ячеек заголовка ячейки (как определено алгоритмом назначения ячеек заголовка). Когда перечисляются ячейки заголовка, пользовательские агенты могут использовать значение атрибутов <LA>abbr</LA> в них, если таковые имеются, вместо содержимого самих ячеек заголовка.
</p>

<ExampleBox>

В этом примере мы видим фрагмент веб-приложения, состоящий из сетки редактируемых ячеек (по сути, простая электронная таблица). Одна из ячеек настроена для отображения суммы ячеек над ней. Три были отмечены как заголовки, в которых используются элементы <LE>th</LE> вместо элементов <LE>td</LE>. Данный скрипт также показывает итоговую сумму.

<Code>
{`
<table>
 <tr>
  <th><input value="Имя">
  <th><input value="Заплатили ($)">
 <tr>
  <td><input value="Jeff">
  <td><input value="14">
 <tr>
  <td><input value="Britta">
  <td><input value="9">
 <tr>
  <td><input value="Abed">
  <td><input value="25">
 <tr>
  <td><input value="Shirley">
  <td><input value="2">
 <tr>
  <td><input value="Annie">
  <td><input value="5">
 <tr>
  <td><input value="Troy">
  <td><input value="5">
 <tr>
  <td><input value="Pierce">
  <td><input value="1000">
 <tr>
  <th><input value="Всего">
  <td><output value="1060">
</table>
`}
</Code>

</ExampleBox>

