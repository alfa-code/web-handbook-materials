<p>
    Элемент <LE>table</LE> представляет данные с более чем одним измерением в форме таблицы.
</p>

<p>
    Элемент <LE>table</LE> участвует в создании таблицы. В таблицах есть строки, столбцы и ячейки, заданные их потомками. Строки и столбцы образуют сетку; ячейки таблицы должны полностью покрывать эту сетку.
</p>


<ExampleBox>

Вот пример <LE>table</LE>, используемой для разметки головоломки судоку. Обратите внимание на отсутствие заголовков, которые не нужны в такой таблице.

<Code>
{`
<style>
		 #sudoku { border-collapse: collapse; border: solid thick; }
		 #sudoku colgroup, table#sudoku tbody { border: solid medium; }
		 #sudoku td { border: solid thin; height: 1.4em; width: 1.4em; text-align: center; padding: 0; }
</style>
<h1>Сегодня судоку</h1>
<table id="sudoku">
		 <colgroup><col><col><col>
		 <colgroup><col><col><col>
		 <colgroup><col><col><col>
		 <tbody>
		  <tr> <td> 1 <td>   <td> 3 <td> 6 <td>   <td> 4 <td> 7 <td>   <td> 9
		  <tr> <td>   <td> 2 <td>   <td>   <td> 9 <td>   <td>   <td> 1 <td>
		  <tr> <td> 7 <td>   <td>   <td>   <td>   <td>   <td>   <td>   <td> 6
		 <tbody>
		  <tr> <td> 2 <td>   <td> 4 <td>   <td> 3 <td>   <td> 9 <td>   <td> 8
		  <tr> <td>   <td>   <td>   <td>   <td>   <td>   <td>   <td>   <td>
		  <tr> <td> 5 <td>   <td>   <td> 9 <td>   <td> 7 <td>   <td>   <td> 1
		 <tbody>
		  <tr> <td> 6 <td>   <td>   <td>   <td> 5 <td>   <td>   <td>   <td> 2
		  <tr> <td>   <td>   <td>   <td>   <td> 7 <td>   <td>   <td>   <td>
		  <tr> <td> 9 <td>   <td>   <td> 8 <td>   <td> 2 <td>   <td>   <td> 5
</table>
`}
</Code>

</ExampleBox>







