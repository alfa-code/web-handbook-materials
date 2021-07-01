<p>
Элемент <LE>cite</LE> указывает на название чего-либо (книга, статья, эссе, стихотворение, песня, сценарий, фильм, телешоу, игра, скульптура, картина, постановка и т.д.) Этим элементом может быть выделена работа, на которую ссылаются или которая цитируется. Может выделяться и работа, о которой упоминают вскользь.
</p>

<p>
Данный элемент не используется для выделения имен людей. В некоторых случаях элеменет <LE>b</LE> может для этого дела. Например, в журналах имена и фамилии людей выделяются, чтобы привлечь максимальное внимание к тому или иному персонажу. При необходимости выделения имен в ряде других случаев используется элемент <LE>span</LE>
</p>

<ExampleBox>

В примере показано типичное использование элемента <LE>cite</LE>

<Code>
{`
<p>
My favorite book is <cite>The Reality Dysfunction</cite> by
Peter F. Hamilton. My favorite comic is <cite>Pearls Before
Swine</cite> by Stephan Pastis. My favorite track is <cite>Jive
Samba</cite> by the Cannonball Adderley Sextet.
</p>
`}
</Code>

</ExampleBox>

<ExampleBox>

Пример верного применения:

<Code>
{`
<p>
According to the Wikipedia article <cite>HTML</cite>, as it
stood in mid-February 2008, leaving attribute values unquoted is
unsafe. This is obviously an over-simplification.
</p>
`}
</Code>

Ниже представлено неверное использование т.к. внутри элемента находится гораздо больше, чем просто название работы.

<!-- do not copy this example, it is an example of bad usage! -->
<p>
According to <cite>the Wikipedia article on HTML</cite>, as it
stood in mid-February 2008, leaving attribute values unquoted is
unsafe. This is obviously an over-simplification.
</p>

</ExampleBox>

<ExampleBox>

Элемент <LE>cite</LE> используется для цитирования в библиографии и для выделения заголовка:

<Code>
{`
<p>
<cite>Universal Declaration of Human Rights</cite>, United Nations,
December 1948. Adopted by General Assembly resolution 217 A (III).
</p>
`}
</Code>

</ExampleBox>

<ExampleBox>

Неправильное использование элемент <LE>cite</LE>, т.к. он не подходит для цитат.

<Code>
{`
<p>
<cite>This is wrong!</cite>, said Ian.
</p>
`}
</Code>

Также неверное употребление т.к. человек - это не название работы:

<Code>
{`
<p>
<q>
This is still wrong!
</q>,
said <cite>Ian</cite>.
</p>
`}
</Code>

Пример правильно построенного предложения без <LE>cite</LE>

<Code>
{`
<p>
<q>
This is correct
</q>, said Ian.
</p>
`}
</Code>

Элемент <LE>b</LE> может выделять имена и ключевые моменты в предложении:

<p>
And then 
<b>
Ian
</b> 
said 
<q>
this might be right, in a
gossip column, maybe!
</q>.
</p>

</ExampleBox>




