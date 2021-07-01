<p>
Элемент <LE>small</LE> представляет собой комментарий, выполненный мелким шрифтом.
</p>

<p>
Элемент <LE>small</LE> не стоит использовать для больших частей текста, например: для абзаца, для создания списка и для разделения текста. Он предназначен для коротких текстов. К примеру, список условий на странице не подойдет для использования данного элемента т.к. текст в списке будет являться главным содержимым страницы, а не дополнением.
</p>

<p>
<LE>small</LE> мы не можем использовать в подзагаловках, для этого подойдет элемент <LE>hgroup</LE> 
</p>

<ExampleBox>

В примере ниже показано при помощи <LE>small</LE>, что НДС не включен в стоимость номера в отеле:

<Code>
{`
<dl>
 <dt>
 	Single room
 <dd>
 	199 € <small>breakfast included, VAT not included</small>
 <dt>
 	Double room
 <dd>
 	239 € <small>breakfast included, VAT not included</small>
</dl>
`}
</Code>

</ExampleBox>

<ExampleBox>

Во втором примере элемент <LE>small</LE> используется для обозначения комментария сбоку в статье.

<Code>
{`
<p>
Example Corp today announced record profits for the
second quarter <small>(Full Disclosure: Foo News is a subsidiary of
Example Corp)</small>, leading to speculation about a third quarter
merger with Demo Group.
</p>
`}
</Code>

В этом примере мы тоже видим боковую панель из статьи, она также имеет мелкий шрифт, указывая на источник информации.

<Code>
{`
<aside>
 <h1>
 Example Corp
</h1>
 <p>
 This company mostly creates small software and Web
 sites.
</p>
 <p>
 The Example Corp company mission is "To provide entertainment
 and news on a sample basis".
</p>
 <p>
 <small>Information obtained from <a href="https://example.com/about.html">example.com</a> home page.</small>
</p>
</aside>
`}
</Code>

</ExampleBox>

<ExampleBox>

В этом примере при помощи <LE>small</LE> выделяется мелким шрифтом важная информация.

<Code>
{`
<p>
<strong>
<small>Continued use of this service will result in a kiss.</small>
</strong>
</p>
`}
</Code>
 
</ExampleBox>


