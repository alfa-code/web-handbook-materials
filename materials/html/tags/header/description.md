<p>
	Элемент <LE>header</LE> представляет собой группу вводных или навигационных средств.
</p>


<ExampleBox>

Вот несколько примеров заголовков. Первый предназначен для игры:

<Code>
{`
<header>
    <p>Добро пожаловать в....</p>
    <h1>Войдворлд!</h1>
</header>
`}
</Code>

В следующем фрагменте показано, как элемент можно использовать для разметки заголовка спецификации:

<Code>
{`
<header>
    <hgroup>
        <h1>Полноэкранный API</h1>
        <h2>Стандарты жизни — Последнее обновление 19 Октября 2015</h2>
    </hgroup>
    <dl>
        <dt>Принять участие</dt>
        <dd><a href="https://github.com/whatwg/fullscreen">GitHub whatwg/fullscreen</a></dd>
        <dt>Commits:</dt>
        <dd><a href="https://github.com/whatwg/fullscreen/commits">GitHub whatwg/fullscreen/commits</a></dd>
    </dl>
</header>
`}
</Code>

</ExampleBox>

<ExampleBox>

В этом примере страница имеет заголовок, заданный элементом <LE>h1</LE>, и два подраздела, заголовки которых заданы элементами <LE>h2</LE>. Содержимое после элемента <LE>header</LE> по-прежнему является частью последнего подраздела, начатого в элементе <LE>header</LE>, поскольку элемент <LE>header</LE> не участвует в алгоритме структуры.

<Code>
{`
<body>
    <header>
        <h1>Little Green Guys With Guns</h1>
        <nav>
            <ul>
                <li><a href="/games">Games</a>
                <li><a href="/forum">Forum</a>
                <li><a href="/download">Download</a>
            </ul>
        </nav>
        <h2>Important News</h2> <!-- this starts a second subsection -->
        <!-- this is part of the subsection entitled "Important News" -->
        <p>To play today's games you will need to update your client.</p>
        <h2>Games</h2> <!-- this starts a third subsection -->
    </header>
    <p>You have three active games:</p>
    <!-- this is still part of the subsection entitled "Games" -->
 ...
`}
</Code>

</ExampleBox>



