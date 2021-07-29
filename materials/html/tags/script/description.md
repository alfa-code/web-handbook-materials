<p>
	 Элемент <LE>script</LE> позволяет авторам включать в свои документы блоки данных. Элемент не представляет контент для пользователя.
</p>

<ExampleBox>

Пример с элементом <LE>script</LE>, используемой при выборке импортированных скриптов, но не других подресурсов:

<Code>
{`
<script referrerpolicy="origin">
    fetch('/api/data');    // не получен с помощью политики <script>
    import('./utils.mjs'); // выбирается с помощью политики <script> (в данном случае "origin")
</script>
`}
</Code>

</ExampleBox>

<ExampleBox>

В этом примере используются два элемента <LE>script</LE>. Один включает внешний классический сценарий, а другой включает некоторые данные в виде блока данных.

<Code>
{`
<script src="game-engine.js"></script>
<script type="text/x-game-map">
........U.........e
o............A....e
.....A.....AAA....e
.A..AAA...AAAAA...e
</script>
`}
</Code>

</ExampleBox>

<ExampleBox>

В следующем примере показано, как можно использовать элемент <LE>script</LE> для определения функции, которая затем используется другими частями документа как часть классического сценария. Он также показывает, как элемент <LE>script</LE> может использоваться для вызова сценария во время анализа документа, в данном случае для инициализации вывода формы.

<Code>
{`
<script>
       function calculate(form) {
         var price = 52000;
         if (form.elements.brakes.checked)
           price += 1000;
         if (form.elements.radio.checked)
           price += 2500;
         if (form.elements.turbo.checked)
           price += 5000;
         if (form.elements.sticker.checked)
           price += 250;
         form.elements.result.value = price;
 }
</script>
        <form name="pricecalc" onsubmit="return false" onchange="calculate(this)">
               <fieldset>
                        <legend>Цена вашей машины</legend>
                        <p>Обычная: £52000.</p>
                        <p>Выбрать дополнительные опции:</p>
                        <ul>
                               <li><label><input type=checkbox name=brakes> Керамические тормоза (£1000)</label></li>
                               <li><label><input type=checkbox name=radio> Радио (£2500)</label></li>
                               <li><label><input type=checkbox name=turbo> Турбо (£5000)</label></li>
                               <li><label><input type=checkbox name=sticker> Наклейка (£250)</label></li>
                        </ul>
                        <p>Всего: £<output name=result></output></p>
               </fieldset>
         <script>
          calculate(document.forms.pricecalc);
 </script>
</form>
`}
</Code>

</ExampleBox>
