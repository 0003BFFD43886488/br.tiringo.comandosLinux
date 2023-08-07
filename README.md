![src$=20230730_134526](https://github.com/notebook-t/notebook-t/assets/140947135/5171d43f-94d2-47f1-8f8b-8cd8d85adaef#alignleft)
El archivo `readme.md` es generalmente utilizado en los proyectos de software para proporcionar información relevante sobre el proyecto. 
Contiene información sobre cómo instalar, configurar y utilizar el software, así como cualquier otro detalle importante que los usuarios o desarrolladores deben conocer. 
Además, el archivo `readme.md` puede incluir información sobre el propósito del proyecto, los requisitos del sistema, las dependencias, los pasos de instalación, la estructura de archivos y directorios, y cualquier otra información relevante que los desarrolladores o usuarios necesiten saber.
Para conocer más a profundidad acerca de este tipo archivo empecemos por el principio.

# Markdown 
Es un lenguaje sencillo, con una sintaxis muy resumida y fácil de recordar e interpretar por humanos, que permite escribir HTML sin la necesidad de usar etiquetas, lo que redunda en velocidad de escritura y facilidad de mantenimiento del contenido. Existen multitud de liberías, para cualquier lenguaje, que permiten convertir el código markdown en HTML y viceversa, por lo que usarlo en cualquier tipo de aplicación es también muy sencillo y directo.
- [Para qué se usa Markdown](https://desarrolloweb.com/home/markdown#track263)
- [Archivos Markdown](https://desarrolloweb.com/home/markdown#track198)
- [Sintaxis](https://desarrolloweb.com/home/markdown#track199)

## Markdown en GitHub para documentar repositorios en el README.md
- [Librería para reconocer Markdown en JavaScrip](https://desarrolloweb.com/home/markdown#track261)
- [notebook-t](https://desarrolloweb.com/home/markdown#track242)
  
> A continuación, se muestran algunos ejemplos de cómo utilizar Markdown en GitHub para agregar formato al archivo README.md:

1. Encabezados: Los encabezados se utilizan para estructurar el contenido y se definen agregando uno o varios símbolos de numeral (#) antes del texto. Por ejemplo:

```
# Título principal
## Título secundario
### Título terciario
```

2. Estilos de texto: Se pueden aplicar estilos a texto como cursiva, negrita o tachado utilizando caracteres especiales. Por ejemplo:

```
*Texto en cursiva*
**Texto en negrita**
~~Texto tachado~~
```

3. Listas: Se pueden crear listas ordenadas utilizando números o listas desordenadas utilizando viñetas. Por ejemplo:

```
1. Primer elemento
2. Segundo elemento
3. Tercer elemento
```

```
- Primer elemento
- Segundo elemento
- Tercer elemento
```

4. Enlaces: Para agregar enlaces a otros sitios web, se utiliza la siguiente sintaxis:

```
[Texto del enlace](URL_del_enlace)
```

Por ejemplo:

```
[Aprende Markdown en GitHub](https://guides.github.com/features/mastering-markdown/)
[~ibarracar0](https://dev.launchpad.net/)
```

5. Imágenes: Para agregar imágenes al archivo README.md, se utiliza la siguiente sintaxis:

```
![Texto alternativo](URL_de_la_imagen)
```

Por ejemplo:

```
![20230730_134526](https://github.com/notebook-t/notebook-t/assets/140947135/5171d43f-94d2-47f1-8f8b-8cd8d85adaef)
```

6. Bloques de código: Para mostrar código de programación, se utiliza la siguiente sintaxis:

```
# Bienvenido/notebooks-group al curso de Diseño de Interiores.

> Nos complace enormemente que hayas decidido unirte a nuestro programa de formación en diseño de interiores. Estamos seguros de que este curso te brindará las herramientas y conocimientos necesarios para desarrollar tus habilidades y alcanzar tus metas en esta apasionante industria.

> Durante las próximas semanas, exploraremos juntos los fundamentos del diseño de interiores, desde los conceptos básicos hasta los aspectos más avanzados de esta disciplina. Aprenderemos sobre los principios del diseño, la selección de colores, la distribución de espacios, los materiales y acabados, entre otros temas relevantes.

> Nuestro equipo de profesionales altamente capacitados y con amplia experiencia en el campo del diseño de interiores estará a tu disposición para brindarte apoyo y orientación durante todo el curso. Además, contarás con acceso a una variedad de recursos, como materiales de lectura, ejercicios prácticos y ejemplos de proyectos reales, que te ayudarán a consolidar tu aprendizaje de manera efectiva.

> Queremos asegurarnos de que aproveches al máximo esta experiencia educativa. Por ello, te animamos a participar activamente en las discusiones en línea, a realizar todas las tareas asignadas y a plantear cualquier duda o inquietud que puedas tener. Nuestro objetivo es que salgas de este curso con una sólida base de conocimientos y la confianza necesaria para aplicarlos en tu futuro profesional.

> Te recordamos que las clases comenzarán el [fecha de inicio]. Asegúrate de tener acceso a la plataforma en línea y revisa el horario de las sesiones para no perderte ninguna clase en vivo. En caso de que no puedas asistir a alguna sesión, todas serán grabadas y estarán disponibles para su visualización posterior.

> Si tienes alguna pregunta antes de que comience el curso, no dudes en comunicarte con nosotros a través de este mismo correo electrónico. Estamos aquí para ayudarte en todo momento.

> Una vez más, te damos la bienvenida a nuestro curso de Diseño de Interiores. Estamos emocionados de conocerte y de acompañarte en este viaje de aprendizaje. ¡Prepárate para sumergirte en el mundo creativo y apasionante del diseño de interiores!

```
Tu código aquí
```shell
bzr push lp:~ibarracar0/+junk/
notebook-t-pach-1 
```

Por ejemplo:

```python
print("Hola, Mundo!")
```

Estos son solo algunos ejemplos básicos de cómo utilizar Markdown en GitHub. Existen muchas más opciones y características disponibles, como tablas, citas, líneas horizontales, entre otros. Para obtener más información sobre el uso de Markdown en GitHub, se puede consultar la guía oficial de GitHub sobre dominio de Markdown.

[Hugo](https://desarrolloweb.com/manuales/manual-de-hugo)

Existe un truco que puedes implementar muy fácilmente basado en selectores de atributo CSS. Te explico.

1.- En el markdown comienzas colocando una imagen normal. Solo que le pones al final de la URL de la imagen una "señal" que indique que la quieres alinear.

![Texto alternativo](https://picsum.photos/400/300#alignleft)

Fíjate que al final de la URL de la imagen hemos colocado #alignleft. Esa finalización en la URL de la imagen, al tratarse de una almohadilla (gato, numeral o como le quieras llamar al caracter "#") no afecta a la URL donde se trata de obtener la imagen en el servidor.

2.- Luego usas un selector de atributo con el valor "$". Estos selectores de atruibuto permiten darle estilos a elementos cuyos atributos casen con determinados valores. El caracter "$" en el nombre del atributo dice a CSS que buscas atributos cutos valores que acaben por determinadas cadenas.

Como tus imagenes que quieres alinear (a la izquierda por ejemplo) todas acabarán en "#alignleft", vamos a buscar justamente valores de atributos src de las imágenes que acaben de esa forma.

El CSS que te sale será algo como esto:

img[src$='#alignleft'] {
	float: left;
  margin: 1rem;
}

Como ves, el selector de atributo "src$" indica que buscas imágenes que tengan al final del atributo src el valor '#alignleft'.

Con eso conseguirás que las imágenes se alineen a la izquierda. Puedes hacer diversos selectores de atributo con este mismo patrón de funcionamiento para hacer imágenes alineadas a la derecha, centradas y todo lo que necesites.

3.- Cómo asignar el CSS personalizado a tu sitio Hugo

Ya luego depende del tema de Hugo que hayas instalado cómo le vas a colocar el CSS personalizado para que se alineen las imágenes.

Lo típico sería que el tema de Hugo tenga un mecanismo para agregarle archivos de CSS con tu propio código que redefinan los estilos del tema. Es cuestión de leer el Readme.

El tema "Tale" que vemos nosotros en el manual de Hugo necesita que le indiques el nombre del archivo CSS que quieres colocar en el tema dentro de la configuración del sitio.

En el archivo hugo.toml colocas:

[Params]
css = ["mi-css.css"]
Luego creas el archivo CSS en el directorio static, que sería la ruta static/mi-css.css. Pero vamos que este tercer punto ya depende mucho del tema y por supuesto si el tema es tuyo propio no deberías tener problema para insertarle el [CSS personalizado](https://developer.mozilla.org/es/play?id=gy4GQrKOQKZAGSdP0T1v1XFN9zl3UTp9ciCHpud5n18xqhmcnRu3LWHdyYj%2BvEZW0nizB7eQ9zE43YYM)
necesario para alinear las imágenes.

```html
<div>
  <div class="uno">CLI:</div>
  <div class="dos">T-Power: Info. <span class="cinco">Artículo: Guía de Markdown en Github</span></div>
  <input class="tres" />
  <textarea class="cuatro"> gapi.load("gapi.iframes:gapi.iframes.style.b</textarea>
</div>

```

```css
.uno {
  color: white;
  background-color: brown;
  margin: 10px;
  width: 50px;
  height: 50px;
  display: inline-block;
}

.dos {
  color: white;
  background-color: black;
  margin: 10px;
  width: 150px;
  height: 70px;
  display: inline-block;
}
.tres {
  color: white;
  background-color: brown;
  margin: 10px;
  width: 75px;
}
.cuatro {
  color: white;
  background-color: brown;
  margin: 10px;
  width: 100px;
}

.cinco {
  background-color: brown;
}

:root {
  --main-bg-color: brown;
}

.uno {
  color: white;
  background-color: var(--main-bg-color);
  margin: 10px;
  width: 50px;
  height: 50px;
  display: inline-block;
}

.dos {
  color: white;
  background-color: black;
  margin: 10px;
  width: 150px;
  height: 70px;
  display: inline-block;
}
.tres {
  color: white;
  background-color: var(--main-bg-color);
  margin: 10px;
  width: 75px;
}
.cuatro {
  color: white;
  background-color: var(--main-bg-color);
  margin: 10px;
  width: 100px;
}

.cinco {
  background-color: var(--main-bg-color);
}

```

```js
class CSS { summoner
  constructor(params) { 
    
  }chatOn 
}
```
