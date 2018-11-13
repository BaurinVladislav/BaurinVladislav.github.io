# TrueConf
A test Site for the company TrueConf.

### Требуется разработать одностраничное приложение (SPA) - эмулятор светофора.
---

#### Приложение должно иметь 3 экрана. Каждый экран представляет из себя модель светофора:
* Экран 1: горит красный (зеленый и желтый тусклые/полупрозрачные)
* Экран 2: горит желтый (зеленый и красный тусклые/полупрозрачные)
* Экран 3: горит зеленый (красный и желтый тусклые/полупрозрачные)

#### Роутинг приложения должен быть настроен таким образом, чтобы при помощи ввода адреса в адресной строке можно было открыть любой из экранов (например,
*	/1 - экран 1,
*	/2 - экран 2,
*	/3 - экран 3)

#### Запуск работы светофора должен происходить только при переходе на корневой адрес приложения (‘/’) 

#### Работа светофора всегда должна начинаться с красного сигнала (экран 1):
*	Красный горит 10 секунд.
*	Желтый - 3 секунды.
*	Зеленый - 15 секунд.

#### Дополнительные задания (бонусное):
*	Реализовать таймер, показывающий сколько секунд осталось до смены сигнала светофора.
*	Реализовать мигание сигнала светофора, если до его смены осталось меньше 3 секунд.

Приложение должно быть написано на фреймворке VueJS и собираться с помощью Webpack.
Приложение не должно иметь глобальных зависимостей. 
Установка должна происходить по команде: "npm install", а запуск - по команде: "npm start". 
Дизайн приложения остается на усмотрение разработчика, ничего сложного не нужно.

---

#### Работа оценивается по следующим критериям:
1.	Соответствие реализации техническому заданию.
2.	Компонентный подход к структуре приложения.
3.	Правильность, чистота и стиль кода.