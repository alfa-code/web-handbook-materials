<p>
 	  Тег <LE>menuitem</LE> определяет элемент команды/меню, который пользователь может вызвать из контекстного меню.
</p>

<p>
	 В настоящее время тег <LE>menuitem</LE> имеет ограниченную поддержку браузерами.
</p>

<ExampleBox>

<Code>
{`
<!DOCTYPE html>
<html>
      <head>
            <title>Пример использования тега <menu></title>
      </head>
      <body>
            <div contextmenu = "testmenu"> 
            Кликни по мне правой кнопкой мыши.
            <menu type = "context" id = "testmenu"> 
                   <menuitem label = "like"></menuitem> 
                   <menuitem label = "dislike"></menuitem> 
            </menu>
            </div>
      </body>
</html>
`}
</Code>

</ExampleBox>










