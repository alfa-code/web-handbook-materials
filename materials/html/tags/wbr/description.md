<p>
	Элемент <LE>wbr</LE> представляет собой возможность разрыва строки. Данным тегом можно определить где именно будут разрывы в слове при переносе на следующую строку.
</p>

<ExampleBox>

В следующем примере цитируется кто-то говорящий, для эффекта это записано одним длинным словом. Однако, чтобы обеспечить читабельность текста, отдельные слова в цитате разделяются элементом <LE>wbr</LE>.

<Code>
{`
<p>Указывая на тигра она прокричала:
"нет<wbr>ни<wbr>одного<wbr>варианта<wbr>для<wbr>тебя<wbr>меня<wbr>поймать<wbr>прямо<wbr>сейчас"!</p>
`}
</Code>

</ExampleBox>

<p>
	Любое содержимое внутри элементов <LE>wbr</LE> не должно считаться частью окружающего текста.
</p>

<ExampleBox>

<Code>
{`
var wbr = document.createElement("wbr");
wbr.textContent = "Это не верно";
document.body.appendChild(wbr);
`}
</Code>

</ExampleBox>



