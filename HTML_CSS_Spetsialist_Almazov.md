* Магия Emmet:

```
div>span.mytext{Текст внутри span}

ul>li*4>a*3

.wrapper>header+main+footer
```
------------

**rectangle** - прямоугольник  
**round**     - круг  
**triangle**  - треугольник  
**solid**     - сплошная линия  
**wrapper**   - обертка

------------

* Прозрачность

```
rgba(255, 255, 255, 0.8)
a - альфаканал
0 - абсолютно прозрачный объект
1 - абсолютно непрозрачный объект
```

-----------------

**Первые 6 строчек, которые надо писать в любом КСС файле. Сброс стилей:**

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

**ctrl+ /**   - закомментирование

------------

# Уровень 1

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