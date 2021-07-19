<p>
	Элемент <LE>thead</LE> представляет собой блок строк, состоящий из столбцов (заголовков) для главного элемента таблицы, если у элемента <LE>thead</LE> есть главный элемент, и это таблица.
</p>

<p>
	Элемент <LE>thead</LE> участвует в создании табличной модели.
</p>

<ExampleBox>

В этом примере показан использование элемента <LE>thead</LE>. Обратите внимание на использование элементов <LE>th</LE> и <LE>td</LE> в элементе <LE>thead</LE>: первая строка - это заголовки, а вторая строка - это объяснение того, как заполнять таблицу.

<Code>
{`
<table>
  <caption> Лист регистрации на школьный аукцион </caption>
  <thead>
  <tr>
      <th><label for=e1>Имя</label>
      <th><label for=e2>Предмет</label>
      <th><label for=e3>Картинка</label>
      <th><label for=e4>Цена</label>
  <tr>
      <td>Ваше имя здесь
      <td>Что продаете?
      <td>Сссылка на картинку
      <td>Цена
 <tbody>
    <tr>
      <td>Ms Danus
      <td>Пончики
      <td><img src="https://example.com/mydoughnuts.png" title="Doughnuts from Ms Danus">
      <td>$45
  <tr>
      <td><input id=e1 type=text name=who required form=f>
      <td><input id=e2 type=text name=what required form=f>
      <td><input id=e3 type=url name=pic form=f>
      <td><input id=e4 type=number step=0.01 min=0 value=0 required form=f>
</table>
<form id=f action="/auction.cgi">
<input type=button name=add value="Submit">
</form>
`}
</Code>

</ExampleBox>

