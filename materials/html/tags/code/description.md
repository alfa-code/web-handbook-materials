<p>
Элемент <LE>code</LE> представляет собой фрагмент компьютерного кода. Это может быть:  XML элемент, имя файла, компьютерная программа или любая другая строка, которую компьютер распознает.
</p>

<p>
Не существует формализованного способа для того, чтобы распознать, какой именно компьютерный код использован. Те пользователи, которые желают выделить <LE>code</LE> элемент при помощи используемого языка, могут использовать атрибут <LE>class</LE>, к примеру, добавить к элементу <LE>class</LE> приставку "language-". 
</p>

<ExampleBox>

В следующем примере показано, как данный элемент можно использовать в абзаце для разметки имен элементов и компьютерного кода, включая знаки препинания.

<Code>
{`
<p>
The <code>code</code> element represents a fragment of computer
code.
</p>

<p>
When you call the <code>activate()</code> method on the
<code>robotSnowman</code> object, the eyes glow.
</p>

<p>
The example below uses the <code>begin</code> keyword to indicate
the start of a statement block. It is paired with an <code>end</code>
keyword, which is followed by the <code>.</code> punctuation character
(full stop) to indicate the end of the program.
</p>
`}
</Code>

</ExampleBox>

<ExampleBox>

В следующем примере показано, как можно разметить блок кода с помощью элементов <LE>pre</LE> и <LE>code</LE>.

<Code>
{`
<pre>
<code class="language-pascal">var i: Integer;
begin
   i := 1;
end.</code>
</pre>
`}
</Code>

В этом примере <LE>class</LE> применяется для обозначения используемого языка.

</ExampleBox>




