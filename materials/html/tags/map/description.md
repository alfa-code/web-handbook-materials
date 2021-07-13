<p>
	Элемент <LE>map</LE> в сочетании с элементом <LE>img</LE> и любыми дочерними элементами <LE>area</LE> показывает карту.
</p>

<p>
	Атрибут <LA>name</LA> дает карте имя, чтобы на нее можно было ссылаться. Атрибут должен присутствовать и иметь непустое значение без пробелов ASCII. Значение атрибута <LA>name</LA> не должно быть равно значению атрибута <LA>name</LA> другого элемента <LE>map</LE> в том же коде. Если также указан атрибут <LA>id</LA>, оба атрибута должны иметь одинаковое значение.
</p>

<p>
	Атрибут <LA>areas</LA> должен возвращать HTMLCollection в <LE>map</LE>, фильтр которого соответствует только элементам <LA>areas</LA>.
</p>

<p>
	<LA>name</LA> должен отражать атрибут содержимого с тем же именем.
</p>

<ExampleBox>

Карты могут быть определены вместе с другим контентом на странице, чтобы упростить восприятие. В этом примере показана страница с картой вверху страницы и соответствующим набором текстовых ссылок внизу.

<Code>
{`
<!DOCTYPE HTML>
<HTML LANG="EN">
<TITLE>Дети: Игрушки</TITLE>
<HEADER>
 	<H1>Игрушки</H1>
	<IMG SRC="/images/menu.gif"
     	 ALT="Babies™ navigation menu. Select a department to go to its page."
      	 USEMAP="#NAV">
</HEADER>
 ...
<FOOTER>
 	<MAP NAME="NAV">
  	<P>
   		<A HREF="/clothes/">Вещи</A>
   		<AREA ALT="Clothes" COORDS="0,0,100,50" HREF="/clothes/"> |
   		<A HREF="/toys/">Игрушки</A>
   		<AREA ALT="Toys" COORDS="100,0,200,50" HREF="/toys/"> |
   		<A HREF="/food/">Еда</A>
   		<AREA ALT="Food" COORDS="200,0,300,50" HREF="/food/"> |
   		<A HREF="/books/">Книги</A>
   		<AREA ALT="Books" COORDS="300,0,400,50" HREF="/books/">
  	</P>
 	</MAP>
</FOOTER>
`}
</Code>

</ExampleBox>




