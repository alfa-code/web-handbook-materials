<p>
	<LE>main</LE> элемент представляет собой главное содержимое документа.
</p>

<p>
	В документе не должно быть более одного <LE>main</LE> элемента, для которого не указан <LA>hidden</LA> атрибут.
</p>

<p>
	Иерархически правильный <LE>main</LE> элемент - это тот, чьи элементы-предки ограничены <LE>html</LE>, <LE>body</LE>, <LE>div</LE>, <LE>form</LE>. Каждый <LE>main</LE> элемент должен быть иерархически правильным <LE>main</LE> элементом.
</p>

<ExampleBox>

В этом примере автор использовал прием, в которой каждый компонент страницы отображается в поле. Чтобы отобразить основное содержимое страницы (в отличие от header, footer, navigation bar, и sidebar), используется <LE>main</LE> элемент.

<Code>
{`
<!DOCTYPE html>
	<html lang="en">
	<title>RPG Система 17</title>
	<style>
 		header, nav, aside, main, footer {
  		margin: 0.5em; border: thin solid; padding: 0.5em;
   		background: #EFF; color: black; box-shadow: 0 0 0.25em #033;
 		}
		h1, h2, p { margin: 0; }
 		nav, main { float: left; }
 		aside { float: right; }
 		footer { clear: both; }
	</style>
	<header>
 		<h1>Система 18</h1>
	</header>
	<nav>
 		<a href="../16/">← Система 17</a>
 		<a href="../18/">RPXIX →</a>
	</nav>
	<aside>
 		<p>В этой системе нет HP mechanic.
	</aside>
	<main>
 		<h2>Создание персонажа</h2>
 		<p>Атрибуты (магия, сила, ловкость) покупаются по цене одного очка за уровень.</p>
 		<h2>Продвижение</h2>
 		<p>При каждой встрече бросайте кубики, чтобы определить все свои навыки. Если вы выбросите больше, чем противник, вы выиграете.</p>
	</main>
	<footer>
		 <p>Copyright © 2013
	</footer>
	</html>
`}
</Code>

В следующем примере используются несколько <LE>main</LE> элементов, и используется сценарий, чтобы заставить навигацию работать без обращения к серверу и установить <LA>hidden</LA> атрибут:

<Code>
{`
<!doctype html>
	<html lang=en-CA>
	<meta charset=utf-8>
	<title> … </title>
	<link rel=stylesheet href=spa.css>
	<script src=spa.js async></script>
	<nav>
 		<a href=/>Домой</a>
 		<a href=/about>О нас</a>
 		<a href=/contact>Контакты</a>
	</nav>
	<main>
 		<h1>Домой</h1>
 	…
	</main>
	<main hidden>
 		<h1>О нас</h1>
	 …
	</main>
	<main hidden>
 		<h1>Контакты</h1>
	…
	</main>
	<footer>Сделано с ❤️ by <a href=https://example.com/>Пример 👻</a>.</footer>
`}
</Code>

</ExampleBox>




