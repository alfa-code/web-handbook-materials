<p>
Элемент <LE>q</LE> показывает цитирование. 
</p>

<p>
Знаки препинания, которые заключают внутрь содержимое элемента, например, кавычки, не ставятся перед, после и внутри <LE>q</LE> элемента. 
</p>

<p>
Содержимое элемента <LE>q</LE> - это цитата из какого-либо источника. Источник указывается с помощью элемента  <LE>cite</LE>
</p>

<p>
Если элемент <LE>cite</LE> присутствует, то ссылка должна быть действительной и отделена пробелами. Сайт может разрешить пользователям переходить по таким ссылкам цитирования, но в первую очередь они предназначены для частного использования, а не для пользователей (к примеру, их используют серверные скрипты, собирающие статистику использования цитат сайтом).
</p>

<p>
Элемент <LE>q</LE> нельзя использовать вместо кавычек, он не представляет собой кавычки в чистом виде. Например, его нельзя использовать для саркастических высказываний.
</p>

<p>
Использование элемента <LE>q</LE> зависит от ситуации. Вы можете ставить знаки препинания без участия данного элемента.
</p>

<ExampleBox>

Простой пример использования элемента <LE>q</LE>

<Code>
{`
<p>
The man said <q>Things that are impossible just take
longer</q>. I disagreed with him.
</p>
`}
</Code>

</ExampleBox>

<ExampleBox>

Пример использования элемента <LE>q</LE> с внешней и внутренней ссылкой:

<Code>
{`
<p>
The W3C page 
<cite>
About W3C
</cite> 
says the W3C's
mission is 
<q cite="https://www.w3.org/Consortium/">To lead the
World Wide Web to its full potential by developing protocols and
guidelines that ensure long-term growth for the Web</q>. 
I disagree with this mission.
</p>
`}
</Code>

</ExampleBox>

<ExampleBox>

В следующем примере цитата находится внутри цитаты:

<Code>
{`
<p>
In 
<cite>
Example One
</cite>
, he writes <q>The man
said <q>Things that are impossible just take longer</q>. I
disagreed with him</q>. Well, I disagree even more!
</p>
`}
</Code>

</ExampleBox>

<ExampleBox>

В следующем примере вместо элемента <LE>q</LE> используются кавычки:

<Code>
{`
<p>
His best argument was ❝I disagree❞, which
I thought was laughable.
</p>
`}
</Code>

</ExampleBox>

<ExampleBox>

В примере ниже кавычки используются для выделения названия. Использование элемена <LE>q</LE> в данном случае было бы неуместным.

<Code>
{`
<p>
The word "ineffable" could have been used to describe the disaster
resulting from the campaign's mismanagement.
</p>
`}
</Code>

</ExampleBox>


