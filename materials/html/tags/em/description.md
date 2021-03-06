<p>
    Элемент <LE>em</LE> акцентирует внимание на своем содержании. Масштаб акцента, который испытывает тот или иной фрагмент, определяеься количеством предыдущих <LE>em</LE> элементтов. Расположение акцента меняет смысл предложения. Таким образом, данный элемент составляет важную часть контента. Эффективный путь использования ударения зависит от языка.
</p>

<ExampleBox>

Данный пример покзывает, как изменеие акцента меняет само предложение. Во-первых, когда мы говорим о каком-либо факте, без акцентирования:

<Code>
{`
<p>
Cats are cute animals.
</p>
`}
</Code>

Когда мы обращаем внимние на первое слово, подразумевается, что речь идет о виде животного (возможно, кто-то полагает, что собаки - милые):

<Code>
{`
<p>
    <em>Cats</em> are cute animals.
</p>
`}
</Code>

Когда мы акцентируем внимание на глаголе, подчеркивается то, что истинность самого предложения может быть сомнительной (возможно, кто-то считает, что кошки не милые):

<Code>
{`
<p>
    Cats <em>are</em> cute animals.
</p>
`}
</Code>

При акценте внимания на прилагательном, мы обращаем внимание на природу кошек (возможно, кто-то думет, что кошки были злыми):

<Code>
{`
<p>
    Cats are <em>cute</em> animals.
</p>
`}
</Code>

Также, если бы кто-то думал, что кошки - это овощи, то можно было бы изменить мнение, выделив даное слово:

<Code>
{`
<p>
    Cats are cute <em>animals</em>.
</p>
`}
</Code>

Если выделить все предложение целиком, то становится понятно, что говорящий максимально пытается передать суть всего предложения. Этот вид акцентирования обычно влияет на пунктуацию, поэтому появляется восклицательный знак:

<Code>
{`
<p>
    <em>Cats are cute animals!</em>
</p>
`}
</Code>

Предложение, содержащее долю гнева одновременно с привлекательностью, может содержать разметку такого типа:

<Code>
{`
<p>
    <em>Cats are <em>cute</em> animals!</em>
</p>
`}
</Code>

</ExampleBox>
