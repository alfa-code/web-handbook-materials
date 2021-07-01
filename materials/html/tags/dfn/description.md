<p>
Элемент <LE>dfn</LE> представляет собой термин или аббревиатуру. Близлежащий абзац, список или раздел к элементу <LE>dfn</LE> должен содержать его расшифровку или описание.
</p>

<p>
Определение термина: если элемент <LE>dfn</LE> имеет атрибут <LE>title</LE>, значит значение атрибута определяется термином. В случае того, когда он содержит в себе только один дочерний элемент и не содержит <LE>text</LE>, то такой дочерний элемент является <LE>abbr</LE> с атрибутом <LE>title</LE>, чем и определяется точное значение данного атрибута. В противном случае термин выдает содержимое элемента <LE>dfn</LE>
</p> 

<p>
Если атрибут <LE>title</LE> находится в <LE>dfn</LE>, то он содержит только определяемый термин. 
</p>

<p>
Элемент <LE>a</LE>, который ссылается на <LE>dfn</LE>, представляет собой термин (он описывается при помощи <LE>dfn</LE>)
</p>

<ExampleBox>

В следующем фрагменте термин "Garage Door Opener" сначала присутствует в первом абзаце, а потом появляется во втором. В обоих случаях по факту отображается только его аббревиатура. 

<Code>
{`
<p>
The <dfn><abbr title="Garage Door Opener">GDO</abbr></dfn>
is a device that allows off-world teams to open the iris.
</p>
<!-- ... later in the document: -->
<p>
Teal'c activated his <abbr title="Garage Door Opener">GDO</abbr>
and so Hammond ordered the iris to be opened.
</p>
`}
</Code>

С помощью элемента <LE>a</LE> ссылку можно сделать заметной:

<Code>
{`
<p>
The <dfn id=gdo><abbr title="Garage Door Opener">GDO</abbr></dfn>
is a device that allows off-world teams to open the iris.
</p>
<!-- ... later in the document: -->
<p>
Teal'c activated his <a href=#gdo><abbr title="Garage Door Opener">GDO</abbr></a>
and so Hammond ordered the iris to be opened.
</p>
`}
</Code>

</ExampleBox>




