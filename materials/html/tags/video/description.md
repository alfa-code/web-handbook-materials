<p>
	Элемент <LE>video</LE> используется для воспроизведения видео или фильмов, а также аудиофайлов с субтитрами.
</p>

<p>
	Контент может быть предоставлен внутри видеоэлемента. Пользовательские агенты не должны показывать это содержимое пользователю; он предназначен для старых веб-браузеров, которые не поддерживают <LE>video</LE>, чтобы можно было опробовать устаревшие плагины для видео или отображать текст для пользователей этих старых браузеров, информирующий их о том, как получить доступ к содержимому видео.
</p>

<p>
	Видеоэлемент - это медиа-элемент, медиа-данные которого якобы являются видеоданными, возможно, со связанными аудиоданными.
</p>

<ExampleBox>

В этом примере показано, как определить, когда видео не воспроизводится правильно:

<Code>
{`
<script>
 function failed(e) {
   // Видеоплеер не работает
   switch (e.target.error.code) {
     case e.target.error.MEDIA_ERR_ABORTED:
       alert('Вы прервали воспроизведение видео.');
       break;
     case e.target.error.MEDIA_ERR_NETWORK:
       alert('Ошибка сети привела к частичному сбою загрузки видео.');
       break;
     case e.target.error.MEDIA_ERR_DECODE:
       alert('Воспроизведение видео было прервано из-за проблемы с повреждением или из-за того, что в видео использовались функции, которые ваш браузер не поддерживал..');
       break;
     case e.target.error.MEDIA_ERR_SRC_NOT_SUPPORTED:
       alert('Видео не может быть загружено либо из-за сбоя сервера или сети, либо из-за того, что формат не поддерживается..');
       break;
     default:
       alert('Неизвестная ошибка.');
       break;
   }
 }
</script>
<p><video src="tgif.vid" autoplay controls onerror="failed(event)"></video></p>
<p><a href="tgif.vid">Загрузить видео</a>.</p>
`}
</Code>

</ExampleBox>








