# Ответы на тестовые вопросы для [FunBox](https://funbox.ru) ( [вакансии "Разработчик HTML/CSS"](https://hh.ru/vacancy/28206274) ).
 Скачать тестовое задание целиком можно здесь: <https://dl.funbox.ru/qt-htmlcss.zip> .
 
 __```P.S. В конце страницы прикреплены ссылки на репозитории с выполненным заданием на GitHub и ссылка на демонстрацию.```__

***

## Level I
> ## ***Q1 - Расскажите, чем, на ваш взгляд, отличается хорошая верстка от плохой с точки зрения:***
> *  ***пользователя;***
> *	 ***менеджера проекта***;
> *	 ***дизайнера***;        
> *	 ***верстальщика***;     
> *	 ***клиентского программиста***;
> *	 ***серверного программиста***.


*  С точки зрения пользователя. 

Важен только конечный продукт и взаимодействие с ним: это нативность использования, то есть сайт/приложение 
выглядит и ведет себя ожидаемо; простое, интуитивно-понятное управление, красота и, одновременно, простота дизайнерских решений; скорость 
отклика, корректное отображение на всех устройствах с разными разрешениями экранов (подробнее об этом можно говорить «вечность»).   
*  С точки зрения менеджера проекта.  

Качественный, понятный код, который было бы просто поддерживать и масштабировать, +, всё то, что
говорилось выше для пользователя, т.к. менеджер берет на себя ответственность в конечном продукте (в отличии от тимллида).
*  С точки зрения дизайнера. 

«Всё выглядит так, как было задумано». Это адаптивность сайта (приложения) под разные устройства, корректность
отображения элементов на разных платформах, разных браузерах (кроссплатформенность), точность в мелочах.
*  С точки зрения верстальщика. 

Понятный, нативный, поддерживаемый код. Это логическое наименование сущностей, грамотная архитектура, 
семантика кода; использование инструментов, фреймворков, упрощающих поддерживаемость кода. 
*  С точки зрения клиентского программиста. 

Примерно то же самое, что и для верстальщика, т.к. для того, чтобы делать клиентскую часть, нужно понимать архитектуру верстки. Интуитивно понятный код и грамотная архитектура (наименование сущностей, классов, ID) ,+ архитектура сайта/приложения с точки зрения производительности, т.к. производительность клиентской части напрямую зависит от производительности самой верстки (сколько ресурсов требует реализованный код)).
* Для серверного программиста.

Производительность кода, т.к. это напрямую влияет на время запросов/ответов с серверной частью (оптимизация изображений и другого
контента, грамотная семантика кода и др.) 

---

> ###  ***Q2 -	Опишите основные особенности верстки крупных многостраничных сайтов, дизайн которых может меняться в процессе реализации и поддержки.***

* Использование систем контроля версий (например, [Github](https://github.com) );
* Хорошая верстка – залог удобства и поддерживаемости (кроссбраузерность, гибкость и продуманность структуры и каркаса сайта, применение 
блочной верстки, а не табличной, грамотность семантики кода);
* Использование современных фреймворков и инструментов, которые: а) увеличивают скорость работы, продуктивность, и б) улучшают 
поддерживаемость проекта ( [Bootstrap](https://getbootstrap.com), [jquery](https://jquery.com), [npm](https://www.npmjs.com), [SASS-SCSS](https://sass-scss.ru) и др.).

> ### ***Расскажите о своем опыте верстки подобных сайтов: какие методологии, инструменты и технологии вы применяли на практике.***

Опыта верстки крупных веб-сайтов не было, не так давно начал изучать технологии веб-разработки. Для практики писал адаптивный, 
кроссплатформенный чат на [Node.js](https://nodejs.org/en/), использовал [npm](https://www.npmjs.com) (для хранения списка всех использованных фреймворков в json и удобной разверстки на др. ПК) и др.). Верстку делал как на чистом HTML/CSS/JS (использовал принцип [флексбоксов](https://html5book.ru/css3-flexbox/) ```#container{display: flex;}``` ), так и на [ejs](http://ejs.co) (шаблонизатор), [jquery](https://jquery.com), [вебсокеты](http://websocket.org) .

---

> ### ***Q3 - Опишите основные особенности верстки сайтов, которые должны одинаково хорошо отображаться как на любом современном компьютере, так и на смартфонах и планшетах под управлением iOS и Android. Расскажите о своем опыте верстки подобных сайтов: какие инструменты и технологии вы применяли, как проверяли результат на различных устройствах, какие именно устройства требовалось поддерживать.***

Уже описывал косвенно в предыдущих вопросах, поэтому просто опишу технологии.

Bootstrap, флекс боксы, медиа запросы ( ```@media all and (orientation: landscape), all and (min-width: 480px) { ... }``` ) (под те
экраны, которые актуальны в настоящий момент), тестирование через обычный браузер Chrome (позволяет сделать тест верстки с эмуляцией 
работы под конкретные устройства от популярных телефонов до планшетов).

---

> ### ***Q4	-	Расскажите, какие инструменты помогают вам экономить время в процессе написания, проверки и отладки кода.***

Написание кода: современные редакторы кода (использую Visual Studio Code) с кучей различных расширений, начиная от, автодополнений 
(таковыми не пользуюсь, учу наизусть всё используемое в коде), заканчивая дебаггингом, современные фреймворки описанные выше.

Проверка и откладка кода: в основном использую возможности браузера Chrome, ПКМ –> исследовать элемент - в большинстве задач достаточно 
для быстрого, гибкого дебаггинга сайта (вывести что-то в лог браузера, изучить сам элемент и «на месте» этим же инструментом пофиксить проблемы со стилями и версткой, и работой скриптов т.к. в режиме реалтайм можно вносить изменения в работу сайта из браузера, отслеживать все события, ресурсы, сеть и производительность, + имеется возможность теста эмуляции на корректность работы с разными устройствами)

Во время работы в нагрузочном тестировании использовал [JMeter](http://jmeter.apache.org), [HP LoadRunner](https://www8.hp.com/sg/en/ad/load-runner/load-runner.html) для теста производительности.

---

> ### ***Q5 - Вам нужно понять, почему страница отображается некорректно в Safari на iOS и в IE на Windows. Код писали не вы, доступа к исходникам у вас нет. Ваши действия? Сталкивались ли вы с подобными проблемами на практике?***

Да, сталкивался при выполнении вашего тестового задания /(^-^)/, но код писал я.

В предложенной ситуации я бы воспользовался встроенными инструментами браузеров для анализа работы страницы, изучил конкретный некорректно отображаемый элемент, как он написан, какие стили использует, в режиме реального времени внес бы изменения в работу сайта через встроенный отладчик браузера и, выявив причину, попытался бы исправить в том же отладчике, убедившись в корректности исправленного решения.

---

> ### ***Q6	-	Дизайнер отдал вам макет, в котором не показано, как должны выглядеть интерактивные элементы при наведении мыши. Ваши действия?***

Уточнить, как должны выглядеть интерактивные элементы при наведении мыши, далее предложить свои варианты.

---

> ### ***Q7 - Какие ресурсы вы используете для развития в профессиональной сфере? Приведите несколько конкретных примеров (сайты, блоги и так далее).***
	
  Подписан на блоги в ВК, телеграмм по тематикам программирования, веб-разработки и front-end (публикации новинок, новостей), [habr](https://habr.com) , подписки на каналы ютуб, читаю книги, просто поиск в гугле, изучаю разные реализованные вещи на [github](github.com) и др.
  
  > ### ***Какое направление развития вам более близко: JS-программирование, HTML/CSS-верстка или и то, и другое?***
 
 И то, и другое.
 
 > ### ***Какие ещё области знаний, кроме тех, что непосредственно относятся к работе, вам интересны?***
 
 Интересен ВЕБ целиком. Начинаю с front-end, далее хочу "уйти" потихоньку в full stack.
 
 ---
 
 > ### ***Q8 -	Расскажите нам о себе и предоставьте несколько ссылок на последние работы, выполненные вами.***
 
Являюсь студентом последнего курса вечернего отделения (работе не мешает), очень хочу заниматься веб-разработкой! На данный момент сам
начал изучение HTML/CSS, JavaScript чистый и его фреймворк Node.js, технологию сокетов, разные модули для нод (использую npm), немного
ознакомился с bootstrap, jquery, ejs. Пишу свой чат для получения практического опыта. Ранее в курсе университета учил C#, C++, C. Во время 
работы в нагрузочном тестировании еще сталкивался с Java со всеми фишками ООП. Так же работал преподавателем GameDev (Unity 3D, Unreal
Engine)
 
Хочу учиться новому, и развиваться вместе с вашей компанией, приносить добро и пользу в этот мир через IT. Очень рад был бы во всём этом 
поучаствовать. 

---

## Level II

> ### ***На этом уровне находится практическое задание, макет к которому вы найдете в том же архиве, что и этот файл. Скачать тестовое задание целиком можно здесь: <https://dl.funbox.ru/qt-htmlcss.zip> .***

### __Ccылка на демонстрацию решения: <https://baurinvladislav.github.io/funbox/SiteCat/> .__

### __Ссылка на репозиторий GitHub с выполненым заданием - <https://github.com/BaurinVladislav/BaurinVladislav.github.io/tree/master/funbox> .__

 __```P.P.S. Отключение продаваемых позиций осуществляется путем присвоения значения true переменным disabledElement1, disabledElement2, disabledElement3 в файле "script.js". Администрирование данного функционала производится пока вручную, при желании можно "повесить" на любой удобный вариант: например, страничка админа```__

---

## Контактные данные
Резюме на [HeadHunter](https://hh.ru): <https://hh.ru/resume/ca1ea0b2ff0409039c0039ed1f476657394145> .

Cтраничка ВК: <https://vk.com/baurinwladik> .

Страничка Телеграм: <https://t.me/BaurinVladislav> .

Почта: <Baurin0@gmail.com>

Телефон: [+7-915-858-35-99](+7-915-858-35-99) (предпочтительный способ связи).
