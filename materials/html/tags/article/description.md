<p>
	Элемент <LE>article</LE> представляет собой самостоятельную часть документа и может использоваться повторно. Это может быть блок сообщения на форуме, статья в журнале, запись в блоге, пользовательский комментарий и так далее. Чаще всего используется в прямом смысле, для обозначения блока содержащего статью.
</p>

<p>
    Когда элементы <LE>article</LE> вложены, внутренние элементы <LE>article</LE> представляют части текта, которые связаны с содержанием главной статьи. Например, запись в блоге на сайте, где можно писать комментарии, отправленные пользователями, может показывать комментарии как элементы <LE>article</LE>, вложенные в элемент <LE>article</LE> для записи в блоге.
</p>

<p>
    Информация об авторе, связанная с элементом <LE>article</LE> (может использоваться элемент <LE>address</LE>), не применяется к вложенным элементам в <LE>article</LE>.
</p>

<p>
    Когда основное содержимое страницы (т.е. исключая нижние колонтитулы, заголовки, блоки навигации и боковые панели) представляет собой единую автономную композицию, это содержимое может быть выделено при помощи <LE>article</LE>, но в таком случае это технически сложно (поскольку элемент существует по себе). - очевидно, что страница должна представлять собой единую композицию, так как это единый документ.
</p>

<ExampleBox>

В этом примере показано сообщение в блоге с использованием элемента <LE>article</LE> с некоторыми комментариями в schema.org:

<Code>
{`
<article itemscope itemtype="http://schema.org/BlogPosting">
    <header>
        <h1 itemprop="headline">Главное правило жизни</h1>
        <p><time itemprop="datePublished" datetime="2009-10-09">з дня назад</time></p>
        <link itemprop="url" href="?comments=0">
    </header>
    <p>
        Представьте, что рядом с вами есть микрофон, он в ожидании того, чтобы вы сказали всему миру то, что думаете. Серьезно.
    </p>
    <p>...</p>
    <footer>
        <a itemprop="discussionUrl" href="?comments=1">Показать комментарии...</a>
    </footer>
</article>
`}
</Code>

Вот тот же пост в блоге, но с некоторыми комментариями:

<Code>
{`
<article itemscope itemtype="http://schema.org/BlogPosting">
    <header>
        <h1 itemprop="headline">Первое правило жизни</h1>
        <p><time itemprop="datePublished" datetime="2009-10-09">3 дня назад</time></p>
        <link itemprop="url" href="?comments=0">
    </header>
    <p>Представьте, что рядом с вами есть микрофон, он в ожидании того, чтобы вы сказали всему миру то, что думаете. Серьезно.</p>
    <p>...</p>
    <section>
        <h1>Комментарии</h1>
        <article itemprop="comment" itemscope itemtype="http://schema.org/UserComments" id="c1">
        <link itemprop="url" href="#c1">
        <footer>
            <p>Написал: <span itemprop="creator" itemscope itemtype="http://schema.org/Person">
                <span itemprop="name">Джордж Вашингтон</span>
                </span>
            </p>
            <p><time itemprop="commentTime" datetime="2009-10-10">15 минут назад</time></p>
        </footer>
        <p>Да! Особенно тогда, когда ты сидишь в гостиной и рассуждаешь с друзьями!</p>
        </article>
        <article itemprop="comment" itemscope itemtype="http://schema.org/UserComments" id="c2">
            <link itemprop="url" href="#c2">
            <footer>
            <p>Написал: <span itemprop="creator" itemscope itemtype="http://schema.org/Person">
                <span itemprop="name">Джордж Хамморд</span>
                </span>
            </p>
            <p><time itemprop="commentTime" datetime="2009-10-10">5 минут назад</time></p>
            </footer>
            <p>Эй, у тебя такое же имя.</p>
        </article>
    </section>
</article>
`}
</Code>

Обратите внимание на использование <LE>footer</LE> для каждого комментария (например, кто его написал и когда): элемент <LE>footer</LE> может появляться в начале раздела, когда это необходимо, как в этом случае. (Использование <LE>header</LE> в этом случае тоже уместно; это вопрос авторских предпочтений.)

</ExampleBox>

<ExampleBox>

В этом примере элементы <LE>article</LE> используются для размещения виджетов на странице портала. Виджеты установлены как настраиваемые встроенные элементы для получения определенного стиля и поведения по сценарию.

<Code>
{`
<!DOCTYPE HTML>
    <html lang=en>
    <title>eHome Portal</title>
    <script src="/scripts/widgets.js"></script>
    <link rel=stylesheet href="/styles/main.css">
    <article is="stock-widget">
        <h1>Stocks</h1>
        <table>
            <thead> <tr> <th> Stock <th> Value <th> Delta
            <tbody> <template> <tr> <td> <td> <td> </template>
        </table>
        <p> <input type=button value="Refresh" onclick="this.parentElement.refresh()">
    </article>
    <article is="news-widget">
        <h1>News</h1>
        <ul>
            <template>
                <li>
                <p><img> <strong></strong>
                <p>
            </template>
        </ul>
        <p> <input type=button value="Refresh" onclick="this.parentElement.refresh()">
    </article>
`}
</Code>

</ExampleBox>






