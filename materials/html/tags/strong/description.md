<p>
Элемент <LE>strong</LE> очень важен для содержимого. 
</p>

<p>
Важно: элемент <LE>strong</LE> используют для заголовков, подзаголовков, абзацев, тем самым выделяя самое важное в содержимом. (Он отличается от элемента <LE>hgroup</LE>, который используется для выделения подзаголовков).
</p>

<ExampleBox>

Например, первое слово в абзаце может быть выделено при помощи <LE>strong</LE>, чтобы акцентировать внимание на фоне остальных слов в тексте. 

</ExampleBox>

<p>
Важно: <LE>strong</LE> можно использовать для обозначения предупреждения или предостережения.
</p>

<p>
Нужно: <LE>strong</LE> элемент следует использовать тогда, когда автор текста желает обратить внимание на что-то в первую очередь.
</p>

<p>
Уровень значимости определенной части контернта во всем тексте определяется наличием предшествующих ранее <LE>strong</LE> элментов в содержимом. Каждый отдельный <LE>strong</LE> элемент увеличивает важность содержимого внутри него.
</p>

<p>
Повышеие значимости отдельной части текста при помощи <LE>strong</LE> элемента не меняет смысл самого предложения.  
</p>

<ExampleBox>

В примере слово "chapter" (глава) явялется частью заголовка, а вкатическое название самой главы выделено <LE>strong</LE>

<Code>
{`
<h1>
	Chapter 1: <strong>The Praxis</strong>
</h1>
`}
</Code>

В следующем примере имя диаграммы в подписи выделено жирным шрифтом, чтобы отличить его от стандартного тексат (до) и подписи (после).

<Code>
{`
<figcaption>
	Figure 1. <strong>Ant colony dynamics</strong>. The ants in this colony are
affected by the heat source (upper left) and the food source (lower right).
</figcaption>
`}
</Code>

Изначально заголовок в данном примере звучит как: "Flowers, Bees, and Honey", но автор решил добавить небольшое дополнение. 
Так <LE>strong</LE> элемент используется для того, чтобы отделить одну часть заголовка от другой. 

<Code>
{`
<h1>
	<strong>Flowers, Bees, and Honey</strong> and other things I don't understand
</h1>
`}
</Code>

</ExampleBox>

<ExampleBox>

Ниже представлен пример предупреждающего сообщения в игре, где различные части выделены в зависимости от того, насколько они важны.

<Code>
{`
<p>
<strong>Warning.</strong> This dungeon is dangerous.
<strong>Avoid the ducks.</strong> Take any gold you find.
<strong><strong>Do not take any of the diamonds</strong>,
they are explosive and <strong>will destroy anything within
ten meters.</strong></strong> You have been warned.
</p>
`}
</Code>
 
</ExampleBox>

<ExampleBox>

В этом примере <LE>strong</LE> используется для обозначения части текста, которую пользователь должен прочитать в первую очередь.

<Code>
{`
<p>
Welcome to Remy, the reminder system.
</p>
<p>
Your tasks for today:
</p>
<ul>
 <li>
 	<p>
 		<strong>Turn off the oven.</strong>
 	</p>
 </li>
 <li>
 	<p>
 	Put out the trash.
 </p>
</li>
 <li>
 	<p>
 	Do the laundry.
 </p>
</li>
</ul>
`}
</Code>

</ExampleBox>
