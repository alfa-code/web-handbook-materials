<p>
	Элемент <LE>footer</LE> представляет нижний колонтитул для его ближайшего дочернего элемента, разделяющего содержимое или корневой элемент. <LE>footer</LE> обычно содержит информацию о своем разделе, например, кто его написал, ссылки на связанные документы, данные об авторских правах и т.д.
</p>

<p>
	Когда элемент <LE>footer</LE> содержит целые разделы, они представляют собой приложения, индексы, подробные лицензионные соглашения и другой подобный контент.
</p>

<p>
	<LE>footer</LE> не обязательно должен появляться в конце раздела, хотя обычно он появляется.
</p>

<p>
	Когда ближайший элемент в содержимом, разделяющий содержимое или корневой элемент, является основным элементом, то он применяется ко всей странице.
</p>

<ExampleBox>

Вот страница с двумя нижними <LE>footer</LE>, один вверху и один внизу, с одинаковым содержанием:

<Code>
{`
<body>
 	<footer><a href="../">Возвращаемся к индексации...</a></footer>
 	<hgroup>
 		<h1>Первопричина</h1>
  		<h2>Значения</h2>
 	</hgroup>
 	<p>
 	Описание процесса.
	</p>
	<footer><a href="../">Возваращемся к индексации...</a></footer>
</body>
`}
</Code>

</ExampleBox>

<ExampleBox>

Вот пример, который показывает, что элемент <LE>footer</LE> используется как для нижнего колонтитула всего сайта, так и для нижнего колонтитула раздела.

<Code>
{`
<!DOCTYPE HTML>
	<HTML LANG="en"><HEAD>
	<TITLE>Ученый - бродяга</TITLE>
	<BODY>
		<H1>Ученый-бродяга</H1>
		<ARTICLE>
 			<H1>Эпизод 15</H1>
 			<VIDEO SRC="/fm/015.ogv" CONTROLS PRELOAD>
 		 		<P><A HREF="/fm/015.ogv">Загрузить видео</A>.</P>
 			</VIDEO>
			<FOOTER> <!-- footer for article -->
 				<P>Published <TIME DATETIME="2009-10-21T18:26-07:00">2009/10/21 в 6:26pm</TIME></P>
 			</FOOTER>
		</ARTICLE>
		<ARTICLE>
 			<H1>Мои любимые тренировки.</H1>
 			<P>Я люблю тренировки.</P>
 			<P>Особенно на свежем воздухе.</P>
 			<FOOTER> <!-- footer for article -->
  				<P>Опубликовано<TIME DATETIME="2009-09-15T14:54-07:00">2009/09/15 в 2:54pm</TIME></P>
 			</FOOTER>
		</ARTICLE>
		<FOOTER> <!-- site wide footer -->
 		<NAV>
  		<P>	<A HREF="/credits.html">Кредиты</A> —
     		<A HREF="/tos.html">Сервисы</A> —
     		<A HREF="/index.html">Блог</A></P>
 		</NAV>
 		<P>Copyright © 2009 Gordon Freeman</P>
		</FOOTER>
	</BODY>
</HTML>
`}
</Code>

</ExampleBox>

<ExampleBox>

Некоторые дизайны сайтов имеют то, что иногда называют «fat footers» - <LE>footer</LE>, которые содержат много материала, включая изображения, ссылки на другие статьи, ссылки на страницы для отправки отзывов, специальные предложения ... в некотором смысле - целое.

Этот фрагмент показывает <LE>footer</LE> на сайте с «fat footers»:

<Code>
{`
...
 <footer>
  	<nav>
   	<section>
   		<h1>Статьи</h1>
    	<p><img src="images/somersaults.jpeg" alt=""> Пойти в спортзал с
    	нашем классом! Наш учитель Джим пйдет с нами. <a href="articles/somersaults/1">Часть
   		1</a> · <a href="articles/somersaults/2">Часть 2</a></p>
    	<p><img src="images/kindplus.jpeg"> Устали ходить <a href="articles/kindplus/1">Читай больше...</a></p>
    	<p><img src="images/crisps.jpeg"> Осталась картошка<a
    	href="articles/crisps/1">Читай больше...</a></p>
  	</section>
   		<ul>
    		<li> <a href="/about">О нас...</a>
    		<li> <a href="/feedback">Оставь обратную связсь!</a>
    		<li> <a href="/sitemap">Карта сайта</a>
   		</ul>
  	</nav>
  	<p><small>Copyright © 2015 The Snacker —
  	<a href="/tos">Сервис</a></small></p>
 </footer>
</body>
`}
</Code>

</ExampleBox>








