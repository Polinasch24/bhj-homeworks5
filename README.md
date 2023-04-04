# Домашнее задание к лекции «Возможности JavaScript в браузере»

Необходимо выполнить и предоставить на проверку следующие задачи

1. [Таймер обратного отсчёта](.countdown)
2. [Игра-кликер](.cookie-clicker)
3. [Игра «Убей кротов»](.mole-game)

Все задачи обязательны к выполнению. Присылать на проверку можно только сразу все три задачи.

Работы должны соответствовать принятому [стилю оформления кода](httpsgithub.comnetology-codecodestyle).

Любые вопросы по решению задач задавайте в группе на Facebook.

## Примечание

В данных задачах и далее по курсу вам потребуется вывод сообщений с помощью
диалоговых окон. Функции alert, prompt и confirm являются частью BOM.
Почитать об их использовании вы можете на следующих ресурсах

1. [Взаимодействие с пользователем alert, prompt, confirm](httpslearn.javascript.ruuibasic)
2. [Window.confirm()](httpsdeveloper.mozilla.orgrudocsWebAPIWindowconfirm)
3. [Window.prompt()](httpsdeveloper.mozilla.orgrudocsWebAPIWindowprompt)
4. [Window.alert()](httpsdeveloper.mozilla.orgrudocsWebAPIWindowalert)

## Бонус

### Книги на курс

1. [DOM Enlightenment](httpdomenlightenment.com)
2. [Eloquent JavaScript](httpseloquentjavascript.net)
3. [DOM Scripting Web Design with JavaScript and the Document Object Model](httpxahlee.infojsscripting_web_index.html)
4. Николас Закас. JavaScript для профессиональных веб-разработчиков

### Скорость загрузки страницы

На лекции мы говорили о принципах построения страницы браузером и двух объектных
моделях DOM и CSSOM.

Для детального понимания, рекомендуем пройти два бесплатных курса 
на udacity от Google (они на английском)

1. [Browser Rendering Optimization](httpsclassroom.udacity.comcoursesud860)
2. [Website Performance Optimization](httpsclassroom.udacity.comcoursesud884)

Илья Григорик, соавтор этих курсов, а также автор большого числа материалов
портала [developers.google.com](httpsdevelopers.google.comwebfundamentals), 
выпустил книгу в 2013 году. Она доступна в формате онлайн совершенно бесплатно по ссылке
[High Performance Browser Networking](httpshpbn.co). Книга рассказывает про
основы сетевого взаимодейтсвия в JavaScript, а также способы повышения
скорости загрузки сайта. Она будет актуальна до  тех пор, пока мы 
используем протокол HTTP версии 1. Для понимания книги вам
понадобится материал всего нашего курса, так как там применяется технология AJAX
(объект XMLHttpRequest), а также там содержится информация, которую вам расскажут
в следующих курсах Нетологии по JavaScript.

На портале [developers.google.com](httpsdevelopers.google.comwebfundamentals)
вы найдёте массу справочной информации, которая поможет ускорить загрузку ваших сайтов.

### События, обработчики событий

Для следующего параграфа вам потребуется больше навыков в задании обработчиков 
событий. Таких способа существует 3. Совсем скоро, через одну лекцию, вы узнаете
об этих особенностях. Но для особо нетерпеливых, почитайте данные статьи

1. [Введение в события DOM](httpsfrontender.infoan-introduction-to-dom-events)
2. [Введение в браузерные события](httpslearn.javascript.ruintroduction-browser-events)
3. [addEventListener vs onclick](httpsstackoverflow.comquestions6348494addeventlistener-vs-onclick6348597#6348597)

### Вызов события программно 

Кстати, событие click можно вызвать вручную! Для этого у найденного элемента имеется
отдельный метод click

```html
button id=push-meAnd then just touch mebutton
```

```javascript
const button = document.getElementById( 'push-me' );

button.onclick = () = alert( 'Till i can get my satisfaction' );

button.click();  Вызовет обработчик click
```

Подробнее смотрите [HTMLElement.click()](httpsdeveloper.mozilla.orgrudocsWebAPIHTMLElementclick)

### defer или async

На лекции вы познакомились с двумя атрибутами тега script - defer и asymc.
Какой из них тогда применять или в каком случае нужен defer, а в каком async
Данные статьи помогают больше понять смысл атрибутов, параллельно рассказывая
о событиях загрузки страницы

1. (script async, defer, async defer, module, nomodule, src, inline)[httpsgist.github.comjakub-g385ee6b41085303a53ad92c7c8afd7a6]
2. (Running Your Code at the Right Time)[httpswww.kirupa.comhtml5running_your_code_at_the_right_time.htm]