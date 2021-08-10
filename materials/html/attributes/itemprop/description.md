<p>
	Атрибут <LA>itemprop</LA> используется для добавления свойств словаря микроданных к элементу. Имя свойства определяется значением <LA>itemprop</LA>, а значение свойства определяется содержимым HTML-элемента, к примеру, текстом который располагается внутри элемента.
</p>

<p>
	Свойство определяется словарём данных. 
</p>

<ExampleBox>

<Code>
{`
<!DOCTYPE html>
<html>
	 <head>
		  <meta charset="utf-8">
		  <title>itemprop</title>
	 </head>
	 <body>
		  <div itemscope itemtype="http://schema.org/Movie">
			   <div>
				    <h1 itemprop="name">Облачный атлас </h1>
				    <span itemprop="alternativeHeadline">Cloud Atlas</span>
				    <img src="http://st.kinopoisk.ru/images/film/464484.jpg" alt="Облачный атлас (Cloud Atlas)" itemprop="image"/>
			   </div>
			   <span>
				    <a itemprop="director" href="/name/23330/">Лана Вачовски</a>,
				    <a itemprop="director" href="/name/26439/">Том Тыквер</a>,
				    <a itemprop="director" href="/name/23329/">Энди Вачовски</a>
			   </span>
			   <span>
				    <a itemprop="producer" href="/name/26437/">Штефан Арндт</a>,
				    <a itemprop="producer" href="/name/31351/">Грант Хилл</a>,
				    <a itemprop="producer" href="/name/26439/">Том Тыквер</a>,
				    <a href="/film/464484/cast/#producer" >и другие</a>.
			   </span>
			   <span>
				    <a itemprop="musicBy" href="/name/312865/">Райнхольд Хайль</a>,
				    <a itemprop="musicBy" href="/name/608605/">Джонни Клаймек</a>,
				    <a itemprop="musicBy" href="/name/26439/">Том Тыквер</a>.
			   </span>
			   <span>
				    <a itemprop="genre" href="/level/10/m_act%5Bgenre%5D/2/">фантастика</a>,
				    <a itemprop="genre" href="/level/10/m_act%5Bgenre%5D/8/">драма</a>,
				    <a itemprop="genre" href="/level/10/m_act%5Bgenre%5D/17/">детектив</a>,
			   </span>  
			   <span class="title">В главных ролях:</span>
			   <div> 
				    <a itemprop="actor" href="/name/9144/">Том Хэнкс</a>
				    <a itemprop="actor" href="/name/1179/">Холли Берри</a>
				    <a itemprop="actor" href="/name/38704/">Джим Броудбент</a>
			   </div>
			   <span itemprop="description">Шесть историй — пять реинкарнаций, 
			    происходящих в разное время,тесно переплетаются между собой…</span>
		  </div>
	 </body>
</html>
`}
</Code>

</ExampleBox>


