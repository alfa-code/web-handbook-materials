<p>
     Элемент <LE>object</LE> может представлять внешний ресурс, который, в зависимости от типа ресурса, будет рассматриваться либо как изображение (как дочерний контекст просмотра), либо как внешний ресурс, который будет обрабатываться плагином.
</p>

<p>
	Элемент <LE>object</LE> задерживает загрузку.
</p>

<p>
	Атрибут <LA>form</LA> используется для связывания элемента <LE>object</LE> с его формой.
</p>


<ExampleBox>
	В этом примере одна страница HTML встроена в другую с помощью элемента <LE>object</LE>.

<Code>
{`
<figure>
	 <object data="clock.html"></object>
	 <figcaption>Мои HTML Часы</figcaption>
</figure>
`}
</Code>

</ExampleBox>

<ExampleBox>

В следующем примере показано, как подключаемый модуль можно использовать в HTML (в данном случае подключаемый модуль Flash для отображения видеофайла). Резервный вариант предоставляется для пользователей, у которых не включен Flash, в этом случае используется элемент <LE>video</LE> для показа видео и предоставления ссылки на видео для тех, у кого нет ни Flash, и не оображается видео в браузере.

<Code>
{`
<p>Это мое видео:
	 <object type="application/x-shockwave-flash">
		  <param name=movie value="https://video.example.com/library/watch.swf">
		  <param name=allowfullscreen value=true>
		  <param name=flashvars value="https://video.example.com/vids/315981">
		  <video controls src="https://video.example.com/vids/315981">
		      <a href="https://video.example.com/vids/315981">Показать видео</a>.
		  </video>
	 </object>
</p>
`}
</Code>

</ExampleBox>










