# Уровень 1

* Магия Emmet:

```
div>span.mytext{Текст внутри span}

ul>li*4>a*3

.wrapper>header+main+footer

a.button{ссылка}*3

ul.menu>li.menu-element*4>a.menu-link

header+nav+main+footer

ul.menu>li.menu-element*4>a.menu-link{Ссылка}

.parent>a.child{Ссылка}
```
------------

**rectangle** - прямоугольник  
**round**     - круг  
**triangle**  - треугольник  
**solid**     - сплошная линия  
**wrapper**   - обертка  
**charset**   - кодировка

------------

* Прозрачность

```
rgba(255, 255, 255, 0.8)
a - альфаканал
0 - абсолютно прозрачный объект
1 - абсолютно непрозрачный объект
```

* Первые 6 строчек, которые надо писать в любом КСС файле. Сброс стилей:

```
    * {
    margin: 0;
    padding: 0;
    border: 0;
    font-size: 0;
    }

```

-------------

Параметр **auto** может быть только у margin-right и margin-left (не у top и bottom).

-------------

**ctrl+ /**   - закомментирование в Visual Studio Code

------------

* Внутренние гиперссылки

    ```
    <a href="#anchor">Это внутренняя ссылка</a>

    Якорь:
    <a name="ancor"></a>
    Слово 'ancor' придумали сами!
    ```

* Псевдоклассы и псевдоэлементы

    ```

    https://codepen.io/nichitenco/pen/zrWBjd

    ```

* Изучение работы со шрифтами, бэкграундом, контейнером, псевдоклассами

    ```
    https://codepen.io/nichitenco/pen/wMmzPo
    ```

* Списки, CSS свойства для списков
    ```
    https://codepen.io/nichitenco/pen/obdgJr
    ```

* Объединение ячеек, заголовки ячеек 

    ```
    https://codepen.io/nichitenco/pen/MKGQqL
    ```

* Табличная верстка

    ```
    https://codepen.io/nichitenco/pen/gPzwPN
    ```


* Формы и их дополнительные атрибуты

    ```
    https://codepen.io/nichitenco/pen/rxvvyG
    ```

* Бэкграунд, отступы внутренние и внешние, закругление углов 

    ```
    https://codepen.io/nichitenco/pen/mVLybo
    ```

* Работа с Koala

```
    Перетаскиваем папку с файлом CSS в программу Коала.
    Щелкаем в программе "Обновить". Должен появиться файл styles.min.css
    Переименовать файл styles.css -> styles.css
    Нажать "обновить" в Коале
    Щелкаем по файлу styles.scss в Koala. Ставим галочку Avtocompile
    Работаем постоянно в файле styles.scss
    В процессе работы Коала самостоятельно будет компилировать его в styles.css и указывать на ошибки
    Файл styles.min.css  сжатый код CSS
```

* HTML5 тэги

```
    <header> Шапка сайта

    <nav> Блок для главного меню

    <aside> Боковая панель

    <main> Основной блок содержимого

    <footer> Подвал сайта

    <article> Статья

    <section> Секция сайта

```

* Light Table - работа с IDE

```
    ctrl пробел  Консоль открыть

    browser      Браузер
    tabset       Дополнительный табсет
    open current file in browser Перенос таба с браузером в табсет

    strl +s      Сохранение
        +r      Обновление браузера

    plugins      Плагины
```

* Резиновая верстка с помощью своейства float (устаревший способ)

    Использована пустышка див-класс "клир", которой заданы свойства clear:both;
    для того чтобы браузер пересчитал все отступы для элементов, лежащих ниже.

```
    https://codepen.io/nichitenco/pen/OMZooy
```

```
    <div class="clear"></div>

    .clear {
    clear:both;
    }

```

* Простая фиксированная двухколоночная верстка

    С помощью отступов слева и справа и задания им свойства "auto" выравниваем 
    двухколоночный шаблон по центру.

```
    https://codepen.io/nichitenco/pen/QyrZpa
```

```
    .wrapper, .header, .footer {

                    width: 960px;

                    margin-left: auto;

                    margin-right: auto;

    }
```
* Свойство display

        https://codepen.io/nichitenco/pen/vLjQXe

```
    * display: inline-block  
    Между элементами появляются пробелы (текстовые "элементы-пустышки")
    Элементы начинают вести себя и как блоки, и как текст (на них применяются
    все блочные и все текстовые свойства)

 ```
 ```
 display: block

    По умолчанию элемент занимает 100% ширины родительского элемента.

    Для того, чтобы выровнять по центру горизонтали блочный элемент, 
    следует задать ему свойства margin-left: auto и margin-right: auto;

    Используется также сокращенная форма margin: 0 auto;
    Работать эти свойства будут в том случае, если ширина будет отлична
    от 100 процентов.
    Иначе блок просто будет занимать 100 прц. ширины. Выравнивать просто
    места не останется.
```
```
* display: inline

    По умолчанию присвоет a, span, b, em
    Элементы следуют друг за другом.
    width и height игнорируются. Его ширина - это ширина содержимого 
    плюс margin border и padding

    margin-top и margin-bottom игнорируются

    Совместно с padding-top и padding-bottom следует корректировать line-height,
    иначе строки будут "наезжать" друг на друга.
```

* Современный метод верстки с помощью свойства display: table

    ```
    https://codepen.io/nichitenco/pen/xZzxLE
    ```
* position

    ```
    position: absolute
    Блоки игнорируют расположение друг друга, и находясь в одном контейнере
    перекрывают друг друга

    position: fixed
    Блок игнорирует всё (в том числе и прокрутку экрана) и позиционируется
    относительно левого верхнего экрана.

    ```
    ```
    position: relative
    Блоки учитывают расположение друг друга.
    Свойства left, top, right, bottom позволяют двигать элемент относительно того
    где он находился. Все свойства используются совместно.
    Сначала задаем position, затем уже left, top, right, bottom.

    Свойство position и свойства left, top, right, bottom так взаимодействуют 
    с другими свойствами:
    absolute - работают 
    fixed - работают
    relative - работают
    static - не работают

    ```

* vertical-aligne  Вертикальное выравнивание
    ```
    Выравнивает элемент по вертикали относительно своего родителя, окружающего текста
    или ячейки таблицы.

    Полезно использовать со свойством display: inline-block для верстки блоков.

    Чтобы несколько горизонтальных блоков выравнились по верхнему краю задают
    vertical-align: top
    ```
* Составные css-свойства
    ```
    border: 1px solid black;

    Аналог:
    border-width: 1px;
    border-style: solid;
    border-color: black;

    border-radius: 10px;

    Аналог:
    border-top-left-radius: 10px;
    border-top-right-radius: 10px;
    border-bottom-left-radius: 10px;
    border-bottom-right-radius: 10px;
    ```
* Практическая работа по верстке. Панель меню в духе Виндовс 8
    ```
    https://codepen.io/nichitenco/pen/dGKGLL
    ```
* Практическая работа по верстке. Четыре квадрата с помощью одного тега div
    ```
    https://codepen.io/nichitenco/pen/xZzOGw

    ```

* Практическая работа. Логоти Майкрософта (четыре квадрата с пробелами между ними)
            с помощью двух тегов div

    ```
    http://codepen.io/nichitenco/pen/bBPVme
    ```
* В каком порядке лучше задавать свойства блоков при верстке:

    ```
    width
    height
    display
    margin
    position
    top/left/right/bottom
    ```

* Тень для текста:
    ```
    text-shadow: 1px 2px 3px yellow;

    1px - смещение по х
    2px - смещение по у
    3px - радиус размытия тени
    yellow - цвет
    ```

* Импорт CSS

    ```
    @import "имя SCSS файла";
    @import "имя SCSS файла";

    Используется для удобства при работе с Коалой.
    ```
```
<canvas> - замена флеша.

WebGL (HTML/CSS/JS) - позволяет отображать трехмерные изображения в браузере. 
Позволяет делать трехмерные браузерные игры.

Unity3D - движок для игр. Можно делать браузерные или атономные игры

WebStorage - локальные базы данных ("продвинуты кукисы")

```
-------

# Уровень 2

* Практическая верстка, квадрат, круг, треугольник в большом прямоугольнике

```
https://codepen.io/nichitenco/pen/OMExKx
```
* Переменные в SCSS

```
$main-width: 800px;
$main-height: 400px;

.rectangle {
	    width: $main-width;
	    heigt: $main-height;		
	    margin-left: $main-width / 2;
	    margin-top: $main-height / 2;
	    margin-left: - ($main-width / 2);
	    margin-top: - ($main-height / 2);
	   }
```
В чистом CSS переменные пока не работают. Только в SCSS.

* Выровняет блоки по верхнему краю:
```
vertical-align: top   
```

* Свойство родительского элемента text-align: center выравнивает блоки по центру по горизонтали.

* Многострочный курсор: 
```
Выбрать символ и нажать ctrl+ d 
``` 

* Сделать картинку круглой:
```
Надо родительскому элементу написать свойства

border-radius: 50%;
overflow: hidden;
```

* Примеси (mixin) в SCSS

```
http://codepen.io/nichitenco/pen/MJaYrY
```

```
@mixin button($height: 80px, $width: 200px) {
		   display: inline-block;
		   margin: 4px;
		   width: $width;
		   height: $heigt;
		   text-align: center;
		   line-height: 80px;
		   border-radius: 4px;
		   text-decoration: none;
		   text-transform: uppercase;
		   font-size: 24 px;
		   border: 1px solide #bcbcbc;
		   box-shadow: 0 0 5px #eee;
}

.simple-button {
		@include button();
		background: lime;
}

.atteneion-button {
		@include button();
		background: yellow;
}

.danger-batton {
		@include button();
		background: red;
		width: 300px;
}
```
* Миксины, общий вид:
```
@mixin имя-примеси($параметр: значение по умолчанию) {
	CSS-свойство: $параметр;
}
```

* Пример подключения миксина:
```
.myclass {
@include имя-примеси(значение);
}
```
```
@include позволяет включить примесь (@mixin) в код CSS
```
* Импорт файла со свойствами SCSS:

```
@import "reset.scss";
или даже
@import "reset";
```
* Сетка, @extend, импорт CSS

```
http://codepen.io/nichitenco/pen/apdgzG
```
* Адаптивная верстка

```
https://codepen.io/nichitenco/pen/egZpZe
```

```
css-tricks.com на сайте есть списки медиазапросов в зависимости от экрана разных моделей.
```

* uilang
```
вкл/выкл
clicking on "button" toggles class "show" on ".menu"

вкл
clicking on "button" adds class "show" on ".menu"

выкл
clicking on "button" removes class "show" on ".menu"
```
* Лайтбокс с помощью скрипта Uilang
```
https://codepen.io/nichitenco/pen/MJjzpy
```
* Адаптивная верстка с помощью миксинов

```
http://codepen.io/nichitenco/pen/jyMjRr
```
unicode-table.com
css-tricks.com
thenewweb.com

css-filters изучить

* Адаптивное выпадающее меню с помощью скрипта Uilang

```
http://codepen.io/nichitenco/pen/mROgwZ
```
* HAML
prepros.io умеет всее что коала + хамл

Gulp/Grunt  консольные инструменты, очень крутые

```
!!!5 доктайп

%html ШТМЛ

/ Комментарий
-#  Комментарий скрытый. Следить, чтобы не вложились теги, лежащие ниже.

%h1 Заголовок

%link{:href=>"styles.css", :rel=>"stylesheet"}

%link{:rel=>"stylesheet", :href=>"styles.css"}
```

еще препроцессоры:

node-webkit (nwjs.io) - NodeJS/Webkit
electron

* nw.js 

Видео 02-4 Уровень 2 расскаывает о работе с nw.js
и создании веб приложений.

* Флексы

flex-start по умолчанию
flex-end все элементы дочерние справа
center  в центре
space-arround с зазором

```
http://codepen.io/nichitenco/pen/vggNYZ
```

# Уровень 3

normalize.css альтернатива CSS

input[type="text"]  Эммет

Префиксами называют технологии, которые еще не вошли в 

* Флексы

justyfy-content свойство, которое задает правило размещения элементов внутри родительского элемента, если они не занимают всю площадь

flex-start
flex-end
center
space-between
space-around