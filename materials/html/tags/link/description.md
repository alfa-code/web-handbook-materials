<p>
 	Элемент <LE>link</LE> позволяет авторам связывать свой документ с другими ресурсами.
</p>

<p>
	Адрес <LE>link</LE> задается атрибутом <LA>href</LA>. Если атрибут <LA>href</LA> присутствует, то его значение должно быть действительным непустым URL-адресом, потенциально окруженным пробелами. Должен присутствовать один или оба атрибута <LA>href</LA>или <LA>imagesrcset</LA>.
</p>

<p>
	Если атрибуты <LA>href</LA> и <LA>imagesrcset</LA> отсутствуют, то элемент не определяет <LE>link</LE>.
</p>

<ExampleBox>

Например, следующий элемент <LE>link</LE> создает две гиперссылки (на одну и ту же страницу):

<Code>
{`
<link rel="author license" href="/about">
`}
</Code>

</ExampleBox>

<ExampleBox>

Эти атрибуты позволяют предварительно загрузить соответствующий ресурс, который позже будет использоваться элементом <LE>img</LE>, который имеет соответствующие значения для его атрибутов <LA>srcset</LA> и <LA>sizes</LA>:

<Code>
{`
<link rel="preload" as="image"
      imagesrcset="wolf_400px.jpg 400w, wolf_800px.jpg 800w, wolf_1600px.jpg 1600w"
      imagesizes="50vw">
<!-- ... Чуть позднее или имеет динамический характер ... -->
<img src="wolf.jpg" alt="A rad wolf"
     srcset="wolf_400px.jpg 400w, wolf_800px.jpg 800w, wolf_1600px.jpg 1600w"
     sizes="50vw">
`}
</Code>

</ExampleBox>

<ExampleBox>

Атрибут <LA>imagesrcset</LA> можно комбинировать с атрибутом <LA>media</LA> для предварительной загрузки соответствующего ресурса, выбранного из источников элемента изображения для художественного оформления:

<Code>
{`
<link rel="preload" as="image"
      imagesrcset="dog-cropped-1x.jpg, dog-cropped-2x.jpg 2x"
      media="(max-width: 800px)">
<link rel="preload" as="image"
      imagesrcset="dog-wide-1x.jpg, dog-wide-2x.jpg 2x"
      media="(min-width: 801px)">
<!-- ... Чуть позднее или имеет динамический характер ... -->
<picture>
  <source srcset="dog-cropped-1x.jpg, dog-cropped-2x.jpg 2x"
          media="(max-width: 800px)">
  <img src="dog-wide-1x.jpg" srcset="dog-wide-2x.jpg 2x"
       alt="An awesome dog">
</picture>
`}
</Code>

</ExampleBox>








