<h1> <b> Содержание заметок. </b> </h1>
1. Коротко о главном <br>
2. Элементы HTML<br>

<hr />
<hr />

<h2> <b> Коротко о главном. </b> </h2>

HTML - язык разместки для web страницы. Он буквально размечает страницу и создаёт макет будущего сайта. 

После создания макета он доводится до ума CSS и получается красиво.

HTML основан на тегах (HTML elements), которые делятся на два типа.

- Теги у которых есть открывающий и закрывающий элемент. Пример:

```html
    <p>
    Пример тег параграфа.
    </p>
```

- Теги без закрывающего элемента или самозакрывающиеся. Пример: 

```html
<!-- Тег строки ввода -->
<input /> 

<!-- Тег для отрисовки картинки -->
<img />
```

Для большинства тегов можно прописать различные параметры внутри. Пример:

```html
<!-- Для тега input параметр value или значение, который помещает текст в строку -->
<input value="It's not a kycok govna" /> 

<!-- Для тега img это параметр src, где хранится ссылка на картинку -->
<img src=" "/>

<!-- Для тега a (тег для встраивания ссылки) это параметр href, где хранится сама ссылка -->
<a href="https://github.com/sanikitin">
		My GitHub.
</a>
```

<b> Важно! </b> Теги принято писать строчными буквами ```<p> </p>```, а не ```<P></P>```. 

<br>

<i> Интересный факт из FreeCodeCamp: Веб-разработчики традиционно используют текст lorem ipsum в качестве текста-заполнителя. Текст Lorem Ipsum случайно взят из знаменитого отрывка Цицерона из Древнего Рима. 

Текст Lorem ipsum использовался в качестве заполнителя текста наборщиками с 16-го века, и эта традиция продолжается в Интернете. </i>

<br>

В HTML можно комментировать код, также, как и в других языках программирования. Для этого нужна следущая конструкция: 

```html
<!-- 
    Тут могла быть ваша реклама.
 -->
```

<p><b> Важно! В VSCode это можно сделать сочетанием клавиш Ctrl + /. </b></p>

Теги можно вкладывать друг в друга. Элемент, который находиться внутри другого HTML элемента называется Inner. Пример: 

```html
<p>
<!-- Тег для ненумерованого списка, явялется Innerом тега параграфа -->
    <ul>
<!-- Элемент списка, явялется Innerом тега списка -->
	    <li>Learn HTML</li>
	    <li>Learn CSS</li>
	    <li>Learn JS</li>
    </ul>
<!-- Тег для нумерованого списка -->
    <ol>
	    <li>Learn HTML</li>
	    <li>Learn CSS</li>
	    <li>Learn JS</li>
    </ol>
</p>
```

<hr />
<hr />

<h2> <b> Элементы HTML. </b> </h2>

<hr />

<h3> <b> Элемент изображения img. </b> </h3>

Синтаксис -  ```<img src="https://www.your-image-source.com/your-image.jpg" alt="Тут я стою такой красивый и смотрю на вас">```

Где src - это атрибут для ссылки на картинку.

Пометки к использованию:

- Использование параметра alt является хорошей практикой. Все элементы img должны иметь атрибут alt. Текст внутри атрибута alt используется для программ чтения с экрана для улучшения доступности и отображается, если изображение не загружается.

- В идеале атрибут alt не должен содержать специальных символов, если в этом нет необходимости.

- Если изображение чисто декоративное, рекомендуется использовать пустой атрибут alt.

</hr>
<hr />

<h3> <b> Элемент ссылки a. </b> </h3>

Синтаксис - ```<a href="https://github.com/sanikitin"> Ссылка на мой GitHub </a>```

Где href - атрибут для ссылки, по которой потом будет переход.

Пометки к использованию: 

- Можно создать внутреннюю ссылку, вы присваиваете атрибут ссылки href хэш-символу # плюс значение атрибута id для элемента, на который вы хотите внутренне ссылаться, обычно дальше вниз по странице. Затем вам нужно добавить тот же атрибут id к элементу, на который вы ссылаетесь. Идентификатор - это атрибут, который уникально описывает элемент. Пример:

```html
<!-- Ссылка -->
<a href="#contacts-header">Contacts</a>

<!-- Куда перенесёт по ссылке -->
<h2 id="contacts-header">Contacts</h2>
```
- Атрибут ```target="_blank"``` позволяет открывать ссылку в новой вкладке.

- Ссылку можно вкладывать в текст или в изображение. Например:

```html
<p>
  Тут будет мой конспект. <a target="_blank" href="https://github.com/sanikitin/Notes_on_HTML"> Ссылка на репозиторий</a> для вас.
</p>
```
- Если указать атрибут ```href="#"```, то ссылка будет активна на сайте, но по ней нельзя будет перейти. Это нужно, если сами ссылки будут в будущем, а сейчас нужна заглушка.

</hr>
<hr />

<h3> <b> Элементы списка. </b> </h3>

Их три вида:
- Ненумерованный список - ```<ul> </ul>```;
- Нумерованный список - ```<ol> </ol> ```;
- Пункт списка - ```<li> </li>```.

</hr>
<hr />

<h3> <b> Элемент ввода input. </b> </h3>

Синтаксис - ```<input type="text">```

Пометки к использованию:
- У элемента может быть задано значение по умолчанию атрибутом ```value=""```.
- Для элемента можно задать надпись на заднем фоне атрибутом ```placeholder=""```.
- Чтобы сделать поле обязательным для заполнения можно добавить атрибут - ```<input type="text" required>```

</hr>
<hr />

<h3> <b> Элемент взаимодействия form. </b> </h3>

Синтаксис - ```<form action="/url-where-you-want-to-submit-form-data"> </form>```

Тег ```<form>``` устанавливает форму на веб-странице. Форма предназначена для обмена данными между пользователем и сервером. 

Пометки к использованию:
- Внутрь формы можно помещать несколько объектов и они будут работать вместе. Например: окно ввода ссылки и кнопка отправки.

```html
<form action="ссылка для отправки на сервер">
    <input type="text" placeholder="место для ссылки">
    <button type="submit">Submit</button>
  </form>
```

</hr>
<hr />

<h3> <b> Элемент кнопки button. </b> </h3>

Синтаксис - ```<button type="submit">Button</button>```

</hr>
<hr />








