<p>
	  Элемент <LE>param</LE> определяет параметры плагинов, вызываемых элементами <LE>object</LE>. Сам по себе он ничего не представляет.
</p>

<p>
   Атрибут <LA>name</LA> показывает имя параметра.
</p>

<p>
   Атрибут <LA>value</LA> дает значение параметра.
</p>

<p>
   Оба атрибута должны присутствовать. Они могут иметь любую <LA>value</LA>.
</p>

<p>
   Если присутствуют оба атрибута и если родительский элемент <LE>param</LE> является элементом <LE>object</LE>, то этот элемент определяет параметр с заданной парой имя-значение.
</p>

<p>
   Если имя или значение параметра, определенного элементом <LE>param</LE>, который является дочерним по отношению к элементу <LE>object</LE>, представляет экземпляр подключаемого модуля и изменяется, и если этот подключаемый модуль обменивается данными с пользовательским агентом с помощью API, который имеет возможность обновлять подключаемый модуль, имя или значение параметра изменяются таким образом, пользовательский агент должен соответствующим образом использовать эту возможность, чтобы уведомить плагин об изменении.
</p>

<p>
   <LA>name</LA> и <LA>value</LA> IDL-атрибутов должны отражать соответствующие атрибуты содержимого с тем же именем.
</p>

<ExampleBox>

В следующем примере показано, как элемент <LE>param</LE> можно использовать для передачи параметра плагину, в данном случае плагину O3D.

<Code>
{`
<!DOCTYPE HTML>
<html lang="en">
     <head>
         <title>O3D</title>
     </head>
     <body>
        <p>
        <object type="application/vnd.o3d.auto">
        <param name="o3d_features" value="FloatingPointTextures">
        <img src="o3d-teapot.png"
          title="3D-иллюстрация чайника, визуализированная с помощью O3D."
          alt="Когда O3D визуализирует чайник, он выглядит как приземистый
           чайник с блестящей металлической отделкой, на которой
           отражается происхлдящее со слабой тенью, вызванной
           освещением.">
        <p>Чтобы увидеть чайник, фактически визуализированный O3D, на вашем
         компьютере, загрузите и установите <a
        href="http://code.google.com/apis/o3d/docs/gettingstarted.html#install">O3D плагин</a>.</p>
        </object>
    <script src="o3d-teapot.js"></script>
        </p>
      </body>
</html>
`}
</Code>

</ExampleBox>

