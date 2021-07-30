<p>
    Элемент <LE>track</LE> позволяет указывать явные внешние синхронизированные текстовые дорожки (`text tracks`) для мультимедийных элементов (`media elements`) <LE>audio</LE> и <LE>video</LE>. Сам по себе он ничего не представляет. Такая дорожка может содержать субтитры на разных языках, различные комментарии и заголовки.
</p>

<ExampleBox>
	
Это видео имеет субтитры на нескольких языках:

<Code>
{`
<video src="brave.webm">
	 <track kind=subtitles src=brave.en.vtt srclang=en label="English">
	 <track kind=captions src=brave.en.hoh.vtt srclang=en label="English for the Hard of Hearing">
	 <track kind=subtitles src=brave.fr.vtt srclang=fr lang=fr label="Français">
	 <track kind=subtitles src=brave.de.vtt srclang=de lang=de label="Deutsch">
</video>
`}
</Code>

</ExampleBox>









