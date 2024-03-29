<p>
	 Элемент <LE>section</LE> представляет собой общий раздел документа или приложения. Раздел в этом контексте представляет собой тематическую группу контента, обычно с заголовком.
</p>

<ExampleBox>

Примерами разделов могут быть главы, различные страницы с вкладками в диалоговом окне с вкладками или пронумерованные разделы диссертации. Домашняя страница веб-сайта может быть разделена на разделы для введения, новостей и контактной информации.

</ExampleBox>

<ExampleBox>

В следующем примере мы видим статью (часть большой веб-страницы) о яблоках, содержащую два коротких раздела.

<Code>
{`
<article>
    <hgroup>
        <h1>Яблоки</h1>
        <h2>ВКУСНЫЕ ФРУКТЫ!</h2>
    </hgroup>
    <p>Яблоки растут на яблоне.</p>
    <section>
        <h1>Красные</h1>
        <p>Часто встречаются в супермаркете.</p>
    </section>
    <section>
         <h1>Зеленые</h1>
         <p>Хороши для яблочного пирога.</p>
    </section>
</article>
`}
</Code>

Обратите внимание, как использование <LE>section</LE> означает, что автор может использовать элементы <LE>h1</LE> повсюду, не беспокоясь о том, находится ли конкретный раздел на верхнем уровне, втором уровне, третьем уровне и так далее.

</ExampleBox>

<ExampleBox>

Вот выпускная программа с двумя разделами: один для списка выпускников, а другой для описания церемонии. (Разметка в этом примере отличается необычным стилем, который иногда используется для минимизации количества межэлементных пробелов.)

<Code>
{`
<!DOCTYPE Html>
<Html Lang=En
 ><Head
   ><Title
     >Церемония награждения выпускников 2022</Title
   ></Head
 ><Body
   ><H1
     >Награждение</H1
   ><Section
     ><H1
       >Церемония</H1
     ><P
       >Открытие</P
     ><P
       >Речь 1</P
     ><P
       >Речь 2</P
     ><P
       >Презентация</P
     ><P
       >Закрытие</P
   ></Section
   ><Section
     ><H1
       >Награждены</H1
     ><Ul
       ><Li
         >Molly Carpenter</Li
       ><Li
         >Anastasia Luccio</Li
       ><Li
         >Ebenezar McCoy</Li
       ><Li
         >Karrin Murphy</Li
       ><Li
         >Thomas Raith</Li
       ><Li
         >Susan Rodriguez</Li
     ></Ul
   ></Section
 ></Body
></Html>
`}
</Code>

</ExampleBox>

<ExampleBox>

В этом примере автор книги разметил некоторые разделы как главы, а некоторые как приложения, и использует CSS, чтобы по-разному стилизовать заголовки в этих двух классах разделов.

<Code>
{`
<style>
    section { border: double medium; margin: 2em; }
    section.chapter h1 { font: 2em Roboto, Helvetica Neue, sans-serif; }
    section.appendix h1 { font: small-caps 2em Roboto, Helvetica Neue, sans-serif; }
</style>
<header>
    <hgroup>
        <h1>Моя книга</h1>
        <h2>Образец с небольшим содержанием</h2>
    </hgroup>
    <p><small>Опубликовано Dummy Publicorp Ltd.</small></p>
</header>
<section class="chapter">
    <h1>Моя первая глава</h1>
    <p>это моя первая глава.</p>
    <p>Но тут два параграфа.</p>
</section>
<section class="chapter">
    <h1>Она включает вторую главу.</h1>
    <p>А,б,в</p>
</section>
<section class="chapter">
    <h1>В главе три будущий пример</h1>
    <p>Похоже на битву.</p>
    <p>Это может разрушить историю.</p>
</section>
<section class="appendix">
    <h1>Дополнительная информация А</h1>
    <p>Показано.</p>
</section>
<section class="appendix">
    <h1>Дополнительная информация Б</h1>
    <p>Ты <em>можешь</em> делать стили.</p>
</section>
`}
</Code>

</ExampleBox>

