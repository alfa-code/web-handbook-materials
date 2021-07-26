<p>
 Элемент <LE>iframe</LE> представляет собой вложенный контекст просмотра.
</p>

<ExampleBox>
  Здесь блог использует атрибут <LA>srcdoc</LA> в сочетании с атрибутом <LA>sandbox</LA>, чтобы предоставить пользователям дополнительный уровень защиты в комментариях к сообщениям блога:

<Code>
{`
<article>
       <h1>У меня есть свой собственный журнал!</h1>
       <p>Я столько усилий приложила для того, чтобы его создать!</p>
       <footer>
                <p>Написано <a href="/users/cap">cap</a>, 1 час назад.
       </footer>
       <article>
                <footer> 13 минут назад, <a href="/users/ch">ch</a> написал: </footer>
                <iframe sandbox srcdoc="<p>уже есть обложка?"></iframe>
       </article>
       <article>
                <footer> 9 минут назад, <a href="/users/cap">cap</a> написал: </footer>
                <iframe sandbox srcdoc="<p>Да, можешь посмотреть <a href=&quot;/gallery?mode=cover&amp;amp;page=1&quot;>в галерее</a>."></iframe>
       </article>
       <article>
                <footer> 5 минут назад, <a href="/users/ch">ch</a> написал: </footer>
                <iframe sandbox srcdoc="<p>это его стол.
              <p>тебе следует earl&amp;amp; поместить меня на следующую страницу."></iframe>
 </article>
`}
</Code>

</ExampleBox>

<ExampleBox>

В этом примере на страницу встроено какое-то совершенно неизвестное, потенциально враждебное HTML-содержимое, предоставленное пользователем. Поскольку он обслуживается из отдельного домена, на него действуют все обычные межсайтовые ограничения. Кроме того, на встроенной странице отключены сценарии, отключены плагины, отключены формы, и она не может перемещаться по фреймам или окнам, кроме своего (или по любым фреймам или окнам, которые он сам встраивает). 

<Code>
{`
<p>Мы вас не боимся! Вот ваш контент, неотредактированный:</p>
<iframe sandbox src="https://usercontent.example.net/getusercontent.cgi?id=12193"></iframe>
`}
</Code>

</ExampleBox>

<ExampleBox>

В этом примере внедрен гаджет с другого сайта. В гаджете включены сценарии и формы, а ограничения исходной <LA>sandbox</LA> сняты, что позволяет гаджету обмениваться данными с исходным сервером. Однако <LA>sandbox</LA> по-прежнему полезна, поскольку отключает плагины и всплывающие окна, тем самым снижая риск того, что пользователь подвергнется воздействию вредоносных программ и других неприятностей.

<Code>
{`
<iframe sandbox="allow-same-origin allow-forms allow-scripts"
        src="https://maps.example.com/embedded.html"></iframe>
`}
</Code>

</ExampleBox>

<ExampleBox>

Предположим, что файл A содержит следующий фрагмент:

<Code>
{`
<iframe sandbox="allow-same-origin allow-forms" src=B></iframe>
`}
</Code>

Файл Б содержит его тоже:

<Code>
{`
<iframe sandbox="allow-scripts" src=C></iframe>
`}
</Code>

Файл В содержит ссылку:

<Code>
{`
<a href=D>Link</a>
`}
</Code>

</ExampleBox>

<ExampleBox>

В этом примере <LE>iframe</LE> используется для встраивания карты из службы онлайн-навигации. Атрибут <LA>allow</LA> используется для включения API геолокации во вложенном контексте.

<Code>
{`
<iframe src="https://maps.example.com/" allow="geolocation"></iframe>
`}
</Code>

</ExampleBox>

<ExampleBox>

Здесь <LE>iframe</LE> используется для встраивания проигрывателя с видеосайта. Атрибут <LA>allowfullscreen</LA> необходим, чтобы проигрыватель мог показывать видео в полноэкранном режиме.

<Code>
{`
<article>
       <header>
               <p><img src="/usericons/1627591962735"> <b>Fred Flintstone</b></p>
               <p><a href="/posts/3095182851" rel=bookmark>12:44</a> — <a href="#acl-3095182851">Приватная публикация</a></p>
       </header>
       <p>Проверь мою новую идею!</p>
       <iframe src="https://video.example.com/embed?id=92469812" allowfullscreen></iframe>
</article>
`}
</Code>

</ExampleBox>

<ExampleBox>

Вот пример страницы, использующей iframe для размещения рекламы от рекламного брокера:

<Code>
{`
<iframe src="https://ads.example.com/?customerid=923513721&amp;format=banner"
        width="468" height="60"></iframe>
`}
</Code>

</ExampleBox>






