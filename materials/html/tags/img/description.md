<p>
 Элемент <LE>img</LE> представляет изображение.
</p>

<p>
Элемент <LE>img</LE> имеет <LA>source</LA> атрибут, изначально установленный для самого элемента.
</p>

<ExampleBox>

<Code>
{`
<img src="1.jpeg" alt="1">
<img src="2.jpeg" loading=eager alt="2">
<img src="3.jpeg" loading=lazy alt="3">
<div id=very-large></div> <!-- Все, что находится после этого div, находится ниже области просмотра -->
<img src="4.jpeg" alt="4">
<img src="5.jpeg" loading=lazy alt="5">
`}
</Code>

</ExampleBox>

<ExampleBox>

Здесь он используется как дополнительный значок:

<Code>
{`
<p>Я живу в <img src="carouge.svg" alt=""> Каорге.</p>
`}
</Code>

</ExampleBox>

<ExampleBox>

Вот еще пример, показывающий одно и то же изображение, используемое в разных контекстах.

<Code>
{`
<article>
       <h1>Мои коты</h1>
       <h2>Флаффи</h2>
       <p>Флаффи - мой любимый.</p>
       <img src="fluffy.jpg" alt="Любит играть с мячиком в саду.">
       <p>Очень мил.</p>
       <h2>Майлз</h2>
       <p>Мой другой кот, только ест и спит.</p>
</article>
`}
</Code>

</ExampleBox>








