<p>
	Элемент <LE>span</LE> сам по себе ничего не значит, но может быть полезен при использовании вместе с глобальными атрибутами, например. <LA>class</LA>, <LA>lang</LA> или <LA>dir</LA>. Он представляет своих потомков.
</p>

<ExampleBox>

В этом примере фрагмент кода размечен с использованием элементов <LE>span</LE> и атрибутов <LA>class</LA>, так что его ключевые слова и идентификаторы могут быть закодированы цветом из CSS:

<Code>
{`
<pre><code class="lang-c"><span class="keyword">for</span> (<span class="ident">j</span> = 0; <span class="ident">j</span> &lt; 256; <span class="ident">j</span>++) {
  <span class="ident">i_t3</span> = (<span class="ident">i_t3</span> & 0x1ffff) | (<span class="ident">j</span> &lt;&lt; 17);
  <span class="ident">i_t6</span> = (((((((<span class="ident">i_t3</span> >> 3) ^ <span class="ident">i_t3</span>) >> 1) ^ <span class="ident">i_t3</span>) >> 8) ^ <span class="ident">i_t3</span>) >> 5) & 0xff;
  <span class="keyword">if</span> (<span class="ident">i_t6</span> == <span class="ident">i_t1</span>)
    <span class="keyword">break</span>;
}</code></pre>
`}
</Code>

</ExampleBox>




