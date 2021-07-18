<p>
	Элемент <LE>source</LE> позволяет авторам указать несколько альтернативных исходных элементов <LE>img</LE> или несколько альтернативных медиаресурсов для медиаэлементов. Сам по себе он ничего не представляет.
</p>

<p>
	Атрибут <LA>type</LA> может присутствовать. Если присутствует, значение должно быть допустимой строкой типа MIME.
</p>

<p>
	Остальные требования зависят от того, является ли родительский элемент элементом <LE>picture</LE> или элементом <LE>media</LE>:
</p>

<p>
	Родительский элемент <LE>source</LE> элемента является элементом <LE>picture</LE>
</p>

<p>
	Атрибут <LA>srcset</LA> должен присутствовать и является атрибутом <LA>srcset</LA>.
</p>

<p>
	Атрибут <LA>srcset</LA> добавляет источники изображений в набор <LE>source</LE>, если выбран исходный элемент.
</p>

<p>
	Если атрибут <LA>srcset</LA> имеет какие-либо изображения, использующие дескриптор ширины, атрибут <LA>sizes</LA> также должен присутствовать. Атрибут <LA>sizes</LA> вносит исходный размер в <LE>source</LE>, если <LE>source</LE> элемент выбран.
</p>

<p>
	Атрибут <LE>media</LE> также может присутствовать. Если присутствует, значение должно содержать действительный список медиа-запросов. Пользовательский агент перейдет к следующему <LE>source</LE> элементу, если значение не соответствует среде.
</p>

<p>
	<LE>source</LE> элемент поддерживает атрибуты измерения. Элемент <LE>img</LE> может использовать атрибуты <LA>width</LA> и <LA>height</LA> <LE>source</LE> элемента вместо атрибутов самого элемента <LE>img</LE> для определения его отображаемых размеров и соотношения сторон, как определено в разделе «Визуализация».
</p>

<p>
	Атрибут <LA>type</LA> показывает тип изображений в <LE>source</LE>, чтобы пользовательский агент мог перейти к следующему элементу <LE>source</LE>, если он не поддерживает данный тип.
</p>

<p>
	Если <LE>source</LE> элемент имеет следующий родственный элемент-<LE>source</LE> или элемент <LE>img</LE> с указанным атрибутом <LA>srcset</LA>, он должен соответствовать хотя бы одному пункту:
</p>

<p>
<ol>
 	<li>Атрибут <LE>media</LE>, указанный со значением, которое после удаления начальных и конечных пробелов ASCII не является пустой строкой и не совпадает с другим элементом без учета регистра символов ASCII для строки «all».</li>
 	<li>Указан <LA>type</LA> атрибут</li>
 	<li>Атрибут <LA>src</LA> не должен присутствовать.</li>
</ol>
</p>

<p>
	Родительский элемент <LE>source</LE> элемента является <LE>media</LE>-элементом
</p>

<p>
	Атрибут <LA>src</LA> показывает URL-адрес медиаресурса. Значение должно быть действительным и непустым URL-адресом, потенциально окруженным пробелами. Этот атрибут должен присутствовать.
</p>

<p>
	Атрибут <LA>type</LA> показывает тип медиаресурса, чтобы помочь пользовательскому агенту определить, может ли он воспроизвести этот медиаресурс перед его включением. Параметр может потребоваться для точного указания способа кодирования ресурса. 
</p>

<ExampleBox>

В следующем списке показаны некоторые примеры использования параметра codecs = MIME в атрибуте <LA>type</LA>.

Видео H.264 с ограниченным базовым профилем (совместимость с основным и расширенным видео) level 3 and Low-Complexity AAC audio in MP4 container

<Code>
{`
	<source src='video.mp4' type='video/mp4; codecs="avc1.42E01E, mp4a.40.2"'>
`}
</Code>

Видео H.264 с расширенным профилем (совместимое с базовыми линиями) level 3 and Low-Complexity AAC audio in MP4 container

<Code>
{`
	<source src='video.mp4' type='video/mp4; codecs="avc1.58A01E, mp4a.40.2"'>
`}
</Code>

H.264 Основной профиль видео level 3 and Low-Complexity AAC audio in MP4 container

<Code>
{`
	<source src='video.mp4' type='video/mp4; codecs="avc1.4D401E, mp4a.40.2"'>
`}
</Code>

Видео H.264 с высоким профилем (несовместимо с основным, базовым или расширенным профилями) level 3 and Low-Complexity AAC audio in MP4 container

<Code>
{`
	<source src='video.mp4' type='video/mp4; codecs="avc1.64001E, mp4a.40.2"'>
`}
</Code>

MPEG-4 Простой визуальный профиль Level 0 video and Low-Complexity AAC audio in MP4 container

<Code>
{`
	<source src='video.mp4' type='video/mp4; codecs="mp4v.20.8, mp4a.40.2"'>
`}
</Code>

MPEG-4 Продвинутый простой профиль Level 0 video and Low-Complexity AAC audio in MP4 container

<Code>
{`
	<source src='video.mp4' type='video/mp4; codecs="mp4v.20.240, mp4a.40.2"'>
`}
</Code>

MPEG-4 Визуальный простой профиль Level 0 video and AMR audio in 3GPP container

<Code>
{`
	<source src='video.3gp' type='video/3gpp; codecs="mp4v.20.8, samr"'>
`}
</Code>

Theora видео and Vorbis аудио in Ogg container

<Code>
{`
	<source src='video.ogv' type='video/ogg; codecs="theora, vorbis"'>
`}
</Code>

Theora видео and Speex аудио in Ogg container

<Code>
{`
	<source src='video.ogv' type='video/ogg; codecs="theora, speex"'>
`}
</Code>

Только Vorbis аудио in Ogg container

<Code>
{`
	<source src='audio.ogg' type='audio/ogg; codecs=vorbis'>
`}
</Code>

Только Speex аудио in Ogg container

<Code>
{`
	<source src='audio.spx' type='audio/ogg; codecs=speex'>
`}
</Code>

Толкьо FLAC аудио in Ogg container

<Code>
{`
	<source src='audio.oga' type='audio/ogg; codecs=flac'>
`}
</Code>

Dirac видео and Vorbis аудио in Ogg container

<Code>
{`
	<source src='video.ogv' type='video/ogg; codecs="dirac, vorbis"'>
`}
</Code>

</ExampleBox>

<p>
	Атрибуты <LA>srcset</LA>, <LA>sizes</LA> и <LA>media</LA> не должны присутствовать.
</p>

<p>
	Если <LE>source</LE> элемент вставлен как дочерний элемент <LA>media</LA> элемента, у которого нет атрибута <LA>src</LA>, а <LE>networkState</LE> которого имеет значение <LE>NETWORK_EMPTY</LE>, пользовательский агент должен вызвать алгоритм выбора ресурса мультимедийного элемента.
</p>

<p>
	Атрибуты IDL <LA>src</LA>, <LA>type</LA>, <LA>srcset</LA>, <LA>sizes</LA> и <LA>media</LA> должны отражать соответствующие атрибуты содержимого с тем же именем. 
</p>

<ExampleBox>

Если автор не уверен, смогут ли все пользовательские агенты отображать предоставленные медиаресурсы, автор может просмотреть  <LE>error</LE> в последнем <LE>source</LE> элементе и произвести резервное копирование:

<Code>
{`
	<script>
 		function fallback(video) {
   		// поставить <video> в контент
   		while (video.hasChildNodes()) {
   		 if (video.firstChild instanceof HTMLSourceElement)
       video.removeChild(video.firstChild);
     	else
       video.parentNode.insertBefore(video.firstChild, video);
   }
   video.parentNode.removeChild(video);
 }
	</script>
	<video controls autoplay>
	<source src='video.mp4' type='video/mp4; codecs="avc1.42E01E, mp4a.40.2"'>
 	<source src='video.ogv' type='video/ogg; codecs="theora, vorbis"'
         onerror="fallback(parentNode)">
 ...
</video>
`}
</Code>

</ExampleBox>



