<h1> <b> Содержание заметок. </b> </h1>
<ol>
	<li> <a href="https://github.com/sanikitin/Notes_on_HTML#--%D0%BA%D0%BE%D1%80%D0%BE%D1%82%D0%BA%D0%BE-%D0%BE-%D0%B3%D0%BB%D0%B0%D0%B2%D0%BD%D0%BE%D0%BC--"> Коротко о главном </a> </li>
	<li> <a href="https://github.com/sanikitin/Notes_on_HTML#--%D1%8D%D0%BB%D0%B5%D0%BC%D0%B5%D0%BD%D1%82%D1%8B-html--"> Элементы HTML </a> </li>
</ol>

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

Ну и в конце нужно понимать основную структуру документа:
```html
<!DOCTYPE html>
<html>
  <head>
    <!-- metadata elements -->
  </head>
  <body>
    <!-- page contents -->
  </body>
</html>
```

В тегах head и body содержится информация о документе, а тег html опоясывает все эти данные для корректного отображения.

В теге head хранится различная информация о HTML-документе для браузера. Например: там подключаются шрифты.

В теге body находится непосредственно разметка страницы.

<hr />
<hr />

<h2> <b> Элементы HTML. </b> </h2>

<ul>
    <li> <a href="https://github.com/sanikitin/Notes_on_HTML#--%D1%8D%D0%BB%D0%B5%D0%BC%D0%B5%D0%BD%D1%82-doctype-html-%D0%B4%D0%BE%D0%BA%D1%83%D0%BC%D0%B5%D0%BD%D1%82%D0%B0--"> Элемент Doctype HTML-документа </a> </li>
    <li> <a href="https://github.com/sanikitin/Notes_on_HTML#--%D1%8D%D0%BB%D0%B5%D0%BC%D0%B5%D0%BD%D1%82-%D0%B8%D0%B7%D0%BE%D0%B1%D1%80%D0%B0%D0%B6%D0%B5%D0%BD%D0%B8%D1%8F-img--"> Элемент изображения img </a> </li>
    <li> <a href="https://github.com/sanikitin/Notes_on_HTML#--%D1%8D%D0%BB%D0%B5%D0%BC%D0%B5%D0%BD%D1%82-%D1%81%D1%81%D1%8B%D0%BB%D0%BA%D0%B8-a--"> Элемент ссылки a </a> </li>
    <li> <a href="https://github.com/sanikitin/Notes_on_HTML#--%D1%8D%D0%BB%D0%B5%D0%BC%D0%B5%D0%BD%D1%82%D1%8B-%D1%81%D0%BF%D0%B8%D1%81%D0%BA%D0%B0--"> Элементы списка </a> </li>
    <li> <a href="https://github.com/sanikitin/Notes_on_HTML#--%D1%8D%D0%BB%D0%B5%D0%BC%D0%B5%D0%BD%D1%82-%D0%B2%D0%B2%D0%BE%D0%B4%D0%B0-input--"> Элемент ввода input </a> </li>
    <li> <a href="https://github.com/sanikitin/Notes_on_HTML#--%D1%8D%D0%BB%D0%B5%D0%BC%D0%B5%D0%BD%D1%82-%D0%B2%D0%B7%D0%B0%D0%B8%D0%BC%D0%BE%D0%B4%D0%B5%D0%B9%D1%81%D1%82%D0%B2%D0%B8%D1%8F-form--"> Элемент взаимодействия form </a> </li>
    <li> <a href="https://github.com/sanikitin/Notes_on_HTML#--%D1%8D%D0%BB%D0%B5%D0%BC%D0%B5%D0%BD%D1%82-%D0%BA%D0%BD%D0%BE%D0%BF%D0%BA%D0%B8-button--"> Элемент кнопки button </a> </li>
    <li> <a href="https://github.com/sanikitin/Notes_on_HTML#--%D1%8D%D0%BB%D0%B5%D0%BC%D0%B5%D0%BD%D1%82-%D0%BA%D0%BE%D0%BD%D1%82%D0%B5%D0%B9%D0%BD%D0%B5%D1%80%D0%B0-div--"> Элемент контейнера div </a> </li>
</ul>

<hr />
<hr />

<h3> <b> Элемент Doctype HTML-документа. </b> </h3>

Синтаксис - 
```html
<!DOCTYPE html>
<html>
  <!-- Your HTML code goes here -->
</html>
```

Большинство основных браузеров поддерживают последнюю спецификацию - HTML5. Однако старые веб-страницы могут использовать предыдущие версии языка.
Поэтому, в начале HTML-документа нужно указывать, что вы используете для корректного считывания. 
Указывать нужно обязательно как в формате выше. 

Затем остальную часть вашего HTML-кода необходимо заключить в теги HTML. Открывающий <html> располагается непосредственно под строкой <! DOCTYPE html>, а закрывающий </html> - в конце страницы.

<hr />
<hr />

<h3> <b> Элемент изображения img. </b> </h3>

Синтаксис -  ```<img src="https://www.your-image-source.com/your-image.jpg" alt="Тут я стою такой красивый и смотрю на вас">```

Где src - это атрибут для ссылки на картинку.

Пометки к использованию:

- Использование параметра alt является хорошей практикой. Все элементы img должны иметь атрибут alt. Текст внутри атрибута alt используется для программ чтения с экрана для улучшения доступности и отображается, если изображение не загружается.

- В идеале атрибут alt не должен содержать специальных символов, если в этом нет необходимости.

- Если изображение чисто декоративное, рекомендуется использовать пустой атрибут alt.

<hr />
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

<hr />
<hr />

<h3> <b> Элементы списка. </b> </h3>

Их три вида:
- Ненумерованный список - ```<ul> </ul>```;
- Нумерованный список - ```<ol> </ol> ```;
- Пункт списка - ```<li> </li>```.

<hr />
<hr />

<h3> <b> Элемент ввода input. </b> </h3>

Синтаксис - ```<input type="text">```

Пометки к использованию:
- У элемента может быть задано значение по умолчанию атрибутом ```value=""```.
- Для элемента можно задать надпись на заднем фоне атрибутом ```placeholder=""```.
- Чтобы сделать поле обязательным для заполнения можно добавить атрибут - ```<input type="text" required>```
- Можно создавать форму для выбора. Кнопки выбора можно также помещать в form, как и button. Пример:
```html
<label for="indoor"> 
  <input id="indoor" type="radio" name="indoor-outdoor">Indoor 
</label>
```
Каждая кнопка выбора (флажок - input) помещается в свой label и автоматически с ним ассоциируется. Все связанные флажки должны иметь одинаковый атрибут name.
Хорошей практикой считается явное связывание input и label. Для label указывается атрибут for, а для input атрибут id. Они должны соотвествовать друг другу.
Пример чекбокса ниже:
```html
<label for="loving"><input id="loving" type="checkbox" name="personality"> Loving</label>
```
Чтобы передавать выбор пользователя в чекбоксах, флажках и input на сервер нужно использовать атрибут value. 
Ниже пример всех трех видов выбора и кнопка отправки данных на сервер.
```html
<form action="https://freecatphotoapp.com/submit-cat-photo">
    <label for="indoor"><input id="indoor" type="radio" name="indoor-outdoor" value="indoor"> Indoor</label>
    <label for="outdoor"><input id="outdoor" type="radio" name="indoor-outdoor" value="outdoor"> Outdoor</label><br>
    <label for="loving"><input id="loving" type="checkbox" name="personality" value="loving"> Loving</label>
    <label for="lazy"><input id="lazy" type="checkbox" name="personality" value="lazy"> Lazy</label>
    <label for="energetic"><input id="energetic" type="checkbox" name="personality" value="energetic"> Energetic</label><br>
    <input type="text" placeholder="cat photo URL" required>
    <button type="submit">Submit</button>
  </form>
```
Можно выставлять какой то флажок или чекбокс по умолчанию с помощью атрибута checked:
```html
<input type="radio" name="test-name" checked>
```
Тут нужно будет разобраться подробнее позже.

<hr />
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

<hr />
<hr />

<h3> <b> Элемент кнопки button. </b> </h3>

Синтаксис - ```<button type="submit">Button</button>```

<hr />
<hr />

<h3> <b> Элемент контейнера div. </b> </h3>

Синтаксис - ```<div> Наполнение </div>```

Элемент div, также известный как элемент подразделения, является контейнером общего назначения для других элементов.

<hr />
<hr />