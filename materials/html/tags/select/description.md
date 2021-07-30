<p>
	 Элемент <LE>select</LE> представляет собой элемент управления для выбора из набора параметров.
</p>

<ExampleBox>

В следующем примере показано, как можно использовать элемент <LE>select</LE>, чтобы предложить пользователю набор параметров, из которых пользователь может выбрать один вариант. Выбран вариант по умолчанию.

<Code>
{`
<p>
     <label for="unittype">Выбрать:</label>
     <select id="unittype" name="unittype">
          <option value="1"> 1 </option>
          <option value="2"> 2 </option>
          <option value="3" selected> 3 </option>
          <option value="4"> 4 </option>
          <option value="5"> 5 </option>
 </select>
</p>
`}
</Code>

Если нет параметра по умолчанию, вместо него можно использовать заполнитель:

<Code>
{`
<select name="unittype" required>
       <option value=""> Выбрать: </option>
       <option value="1"> 1 </option>
       <option value="2"> 2 </option>
       <option value="3"> 3 </option>
       <option value="4"> 4 </option>
       <option value="5"> 5 </option>
</select>
`}
</Code>

</ExampleBox>

<ExampleBox>

Здесь пользователю предлагается набор опций, из которых он может выбрать любое количество. По умолчанию выбраны все пять параметров.

<Code>
{`
<p>
     <label for="allowedunits">Выбрать:</label>
     <select id="allowedunits" name="allowedunits" multiple>
      <option value="1" selected> 1 </option>
      <option value="2" selected> 2 </option>
      <option value="3" selected> 3 </option>
      <option value="4" selected> 4 </option>
      <option value="5" selected> 5 </option>
 </select>
</p>
`}
</Code>

</ExampleBox>

<ExampleBox>

Иногда пользователю нужно выбрать один или несколько элементов. В этом примере показан такой интерфейс.

<Code>
{`
<label>
     Выбрать песню:
     <select multiple required name="act2">
      <option value="s1">It Sucks to Be Me (Reprise)
      <option value="s2">There is Life Outside Your Apartment
      <option value="s3">The More You Ruv Someone
      <option value="s4">Schadenfreude
      <option value="s5">I Wish I Could Go Back to College
      <option value="s6">The Money Song
      <option value="s7">School for Monsters
      <option value="s8">The Money Song (Reprise)
      <option value="s9">There's a Fine, Fine Line (Reprise)
      <option value="s10">What Do You Do With a B.A. in English? (Reprise)
      <option value="s11">For Now
     </select>
</label>
`}
</Code>

</ExampleBox>
