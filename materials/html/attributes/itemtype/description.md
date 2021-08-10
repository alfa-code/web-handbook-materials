<p>
	Атрибут <LA>itemtype</LA> указывает адрес словаря, который будет применяться для определения свойств элемента в структуре данных. 
</p>

<p>
	В качестве значения принимается адрес страницы словаря.
</p>

<ExampleBox>

<Code>
{`
<!DOCTYPE html>
<html>
	 <head>
		  <meta charset="utf-8">
		  <title>itemtype</title>
	 </head>
	 <body>
		  <div itemscope itemtype="http://schema.org/Organization">
			   <span itemprop="name">Яндекс</span>
			   Контакты:
			    <div itemprop="address" itemscope itemtype="http://schema.org/PostalAddress">
				     Адрес:
				      <span itemprop="streetAddress">Льва Толстого, 16</span>
				      <span itemprop="postalCode"> 119021</span>
				      <span itemprop="addressLocality">Москва</span>,
			    </div>
			   Телефон:<span itemprop="telephone">+7 495 739–70–00</span>,
			   Факс:<span itemprop="faxNumber">+7 495 739–70–70</span>,
			   Электронная почта: <span itemprop="email">pr@yandex-team.ru</span>
		  </div>
	 </body>
</html>
`}
</Code>

</ExampleBox>


