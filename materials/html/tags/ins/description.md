<p>
	Элемент <LE>ins</LE> представляет собой дополнение к документу.
</p>

<ExampleBox>

Ниже показано дополнение к абзацу:

<Code>
{`
<aside>
 	<ins>
 		<p> Я люблю фрукты. </p>
 	</ins>
</aside>
`}
</Code>

Далее в примере то же самое, потому что все, что в элементе <LE>aside</LE> считается phrasing content и, следовательно, - только один абзац:

<Code>
{`
<aside>
 	<ins>
 		Яблоки <em>вкусные</em>.
 	</ins>
 	<ins>
 		И груши.
 	</ins>
</aside>
`}
</Code>

</ExampleBox>

<p>
    Элементы <LE>ins</LE> не должны пересекать подразумеваемые границы абзаца.
</p>

<ExampleBox>

В следующем примере представлены два абзаца, второй из которых состоит из двух частей. Таким образом, первый элемент <LE>ins</LE> в этом примере пересекает границу абзаца, что плохо.

<Code>
{`
<aside>
	 <!-- Не делайте так -->
 	<ins datetime="2005-03-16 00:00Z">
  	<p> Я люблю фрукты. </p>
  		Яблоки <em>вкусные</em>.
 	</ins>
 	<ins datetime="2007-12-19 00:00Z">
  		И груши.
 	</ins>
</aside>
`}
</Code>

Ниже лучший способ. Тут больше элементов, но ни один из элементов не пересекает подразумеваемые границы абзаца.

<Code>
{`
<aside>
 	<ins datetime="2005-03-16 00:00Z">
  	<p> Я люблю фрукты. </p>
 	</ins>
 	<ins datetime="2005-03-16 00:00Z">
 		 Яблоки <em>вкусные</em>.
 	</ins>
 	<ins datetime="2007-12-19 00:00Z">
  		И груши.
 	</ins>
</aside>
`}
</Code>

</ExampleBox>



