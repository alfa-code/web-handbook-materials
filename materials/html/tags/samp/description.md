<p>
	Элемент <LE>samp</LE> представляет собой знак или подпись авторства, принадлежащий другой программе или компьютерной системе.
</p>

<ExampleBox>

В следующем примере элемент <LE>samp</LE> встроен:

<Code>
{`
<p>
	Компьютер напсиал <samp>Слишком много сыра на втором подносе</samp>, но я не знаю, что это значит.
</p>
`}
</Code>

</ExampleBox>

<ExampleBox>

Во втором примере показан блок выходных данных консольной программы. Вложенные элементы <LE>samp</LE> и <LE>kbd</LE> позволяют стилизовать определенные элементы образца вывода с помощью таблицы стилей. Также есть несколько частей шаблона, которые содержат еще более подробную разметку. Для этого используются элементы <LE>span</LE>.

<Code>
{`
<pre>
	<samp>
		<span class="prompt">jdoe@mowmow:~$</span> <kbd>ssh demo.example.com</kbd>
		Last login: Tue Apr 12 09:10:17 2005 from mowmow.example.com on pts/1
		Linux demo 2.6.10-grsec+gg3+e+fhs6b+nfs+gr0501+++p3+c4a+gr2b-reslog-v6.189 #1 SMP Tue Feb 1 11:22:36 PST 2005 i686 unknown
		<span class="prompt">jdoe@demo:~$</span>
		<span class="cursor">_</span>
	</samp>
</pre>
`}
</Code>

</ExampleBox>

<ExampleBox>

Третий пример показывает блок ввода и соответствующий ему вывод. В примере используются элементы как <LE>code</LE>, так и <LE>samp</LE>.

<Code>
{`
<pre>
	<code class="language-javascript">console.log(2.3 + 2.4)</code>
	<samp>4.699999999999999</samp>
</pre>
`}
</Code>

</ExampleBox>


