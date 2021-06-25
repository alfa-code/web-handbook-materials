<p>
    Если элемент <LinkElement>a</LinkElement> имеет атрибут href, то он представляет собой гиперссылку (гипертекстовую привязку), помеченную ее содержимым.
</p>

<p>
    Если элемент <LinkElement>a</LinkElement> не имеет атрибута href, тогда элемент представляет собой заполнитель, где в противном случае могла бы быть размещена ссылка, если бы она была релевантной, состоящая только из содержимого элемента.
</p>

<p>
    Атрибуты target, download, ping, rel, hreflang, type, и referrerpolicy не должны использоваться, если атрибут href отсутствует.
</p>

<p>
    Если атрибут itemprop указан в элементе <LinkElement>a</LinkElement>, то необходимо также указать атрибут href.
</p>

<ExampleBox>
    Если сайт использует единую панель навигации на каждой странице, то ссылка, которая обычно ведет на саму страницу (тукущую), может быть размечена с помощью элемента <LinkElement>a</LinkElement> без атрибута <LinkAttribute>href</LinkAttribute>:

    <Code>
{`<nav>
    <ul>
        <li> <a href="/">Home</a> </li>
        <li> <a href="/news">News</a> </li>
        <li> <a>Examples</a> </li>
        <li> <a href="/legal">Legal</a> </li>
    </ul>
</nav>`}
    </Code>

</ExampleBox>
