<p>
	 Элемент <LE>nav</LE> представляет собой раздел страницы, который ссылается на другие страницы или части страницы: раздел с навигационными ссылками.

<ExampleBox>

В следующем примере есть два элемента <LE>nav</LE>: один для основной навигации по сайту, а другой для дополнительной навигации по самой странице.

<Code>
{`
<body>
 	<h1>Вики центр</h1>
 	<nav>
 		 <ul>
   			<li><a href="/">Домой</a></li>
   			<li><a href="/events">Текущие мероприятия</a></li>
   		...более...
  		</ul>
 	</nav>
 	<article>
 	<header>
   		<h1>Демоны</h1>
   		<p>Написано А.Н.Азером</p>
  	</header>
  	<nav>
  		 <ul>
   			 <li><a href="#public">Демонстрации</a></li>
    		<li><a href="#destroy">Разбор</a></li>
    	...более...
   		</ul>
  	</nav>
  	<div>
   	<section id="public">
   		 <h1>Демонстрации</h1>
   		 <p>...более...</p>
   	</section>
   	<section id="destroy">
  		 <h1>Разбор</h1>
   	<p>...более...</p>
  	</section>
  	 ...более...
  	</div>
  	<footer>
  		 <p><a href="?edit">Дополнения</a> | <a href="?delete">Удалить</a> | <a href="?Rename">Переименовать</a></p>
  	</footer>
 	</article>
 	<footer>
  		<p><small>© copyright 1998 Exampland Emperor</small></p>
 	</footer>
</body>
`}
</Code>

</ExampleBox>

<ExampleBox>

В следующем примере на странице есть несколько мест, где присутствуют ссылки, но только одно из этих мест считается разделом навигации.

<Code>
{`
<body itemscope itemtype="http://schema.org/Blog">
 <header>
  	<h1>Проснись!</h1>
  	<p><a href="news.html">Новости</a> -
    	<a href="blog.html">Блог</a> -
    	<a href="forums.html">Форум</a></p>
 	<p>Последнее изменение: <span itemprop="dateModified">2009-04-01</span></p>
 	<nav>
  	<h1>Навигация</h1>
  		 <ul>
   			 <li><a href="articles.html">Статьи</a></li>
   			 <li><a href="today.html">Нужно проснуться сегодня</a></li>
   			 <li><a href="successes.html">Кого нужно разбудить</a></li>
   		</ul>
  	</nav>
 </header>
 	<main>
  	<article itemprop="blogPosts" itemscope itemtype="http://schema.org/BlogPosting">
   	<header>
   		 <h1 itemprop="headline">Мой день на пляже</h1>
   	</header>
  		 <div itemprop="articleBody">
   		 <p>Сегодня я ходил на пляж и было очень весело.</p>
    	...больше информации...
   		 </div>
  	<footer>
   		 <p>Выложено<time itemprop="datePublished" datetime="2009-10-10">Четверг</time>.</p>
   	</footer>
  	</article>
  	...больше постов в блоге...
	 </main>
 	<footer>
  		<p>Copyright ©
  		<span itemprop="copyrightYear">2010</span>
   		<span itemprop="copyrightHolder">The Example Company</span>
  		</p>
  		<p><a href="about.html">О нас</a> -
     		<a href="policy.html">Права</a> -
    		<a href="contact.html">Связаться с нами</a></p>
	</footer>
</body>
`}
</Code>

Вы также можете увидеть описание данных в приведенном выше примере, которые используют словарь schema.org для предоставления даты публикации и других метаданных о сообщении в блоге.

</ExampleBox>

<ExampleBox>

Элемент <LE>nav</LE> не обязательно должен содержать список, он также может содержать другие типы контента. В этом блоке навигации ссылки представлены в прозе:

<Code>
{`
<nav>
 	<h1>Навигация</h1>
 	<p>Вы на моей домашней странице. Слева <a href="/blog">мой блог</a>, справа вы можете  увидеть множество <a
 	href="/school">школьных материалов</a> все школьные материалы представлены тезисно <a href="/school/thesis">тезисы</a>.</p>
 	<p>очень смешно выглядит табличка<a
 	href="https://games.example.com/">"игры"</a>. более скучно выглядит <a
 	href="https://isp.example.net/">ISP™</a>.</p>
 	<p>темновато выглядит<a href="/about">свяжитесь с нами</a>. если вы увидете крысу, срочно закройте страничку</p>
</nav>
`}
</Code>

</ExampleBox>

<ExampleBox>

В этом примере в почтовом приложении используется <LE>nav</LE>, позволяющая пользователю переключать папки:

<Code>
{`
<p><input type=button value="Compose" onclick="compose()"></p>
<nav>
 	<h1>Папки</h1>
	<ul>
 		 <li> <a href="/inbox" onclick="return openFolder(this.href)">Inbox</a> <span class=count></span>
  		<li> <a href="/sent" onclick="return openFolder(this.href)">Sent</a>
  		<li> <a href="/drafts" onclick="return openFolder(this.href)">Drafts</a>
  		<li> <a href="/trash" onclick="return openFolder(this.href)">Trash</a>
  		<li> <a href="/customers" onclick="return openFolder(this.href)">Customers</a>
	</ul>
</nav>
`}
</Code>

</ExampleBox>

