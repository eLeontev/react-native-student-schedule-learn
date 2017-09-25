# Разработка мобильного приложение на React Native

## Введение
В ходе воркшопа мы освоим основы разработки мобильного приложения на `JavaScript` с использованием библиотеки `React Native`.
Мы начнем с изучения основ библиотек `React` и `React Native`, затем создадим свой компонент для отображения расписания, а в конце мы стилизуем этот компонент как вам понравится.

## Необходимое ПО
Для написания мобильного приложения на `React Native` вам понадобяться `Node.js`, `npm`, `git` и удобный редактор кода.

### Установка `Node.js`
Для начала, можно проверить, уставлен ли `Node.js`. Для этого в консоли/терминале необходимо ввести команду `node -v`.
Если ответ был похож на
```
node -v
v7.7.1
```
то `Node.js` установлен. Если же ответ другой, например, там написано, что невозможно найти команду `node`, то придется установить самому.

Скачать и установить `Node.js` можно с [официальной страницы](https://nodejs.org/en/)

### Установка `npm`
Вообще, `npm` устанавливается вместе с `Node.js`, так что если `Node.js` установлен, то и `npm` установлен, скорей всего.
Что бы проверить можно ввести команду в консоли/терминале `npm -v`. Если в ответе будет версия `npm`, то все в порядке, если нет - нужно переустановить `Node.js`.

### Установка `git`
По примеру с программами выше проверить установку можно командой `git --version`. Если же необходимо установить, то сделать это можно с [официальной страницы](https://git-scm.com/download/).

### Установка редактора кода
Хорошими редакторами для учебных целей являются [VS Code](https://code.visualstudio.com/) или [Atom](https://atom.io/), но вы можете выбрать свой.

### А вообще...
А вообще, если находитесь в классе со всеми, то мы уже все установили и проверили. Шаги выше необходимо пройти, если вы делаете, например, из дома.

## React
Библиотека для создания интерактивных веб-сайтов от кампании Facebook. Наименьшей единицей для работы с этой библиотекой являются компоненты - объекта языка `JavaScript`, с которыми удобно работать и представлять в виде традиционного `HTML` и которые содержат в себе и описание внешнего вида и код для обработки взаимодействия пользователя и этого компонента. Именно благодаря данному подходу построения приложений получилось сделать так, что бы эти компоненты превращались не только в `HTML`, но и в приложения.

## JSX (JavaScript extended)
`JSX` - это надстройка над языком `JavaScript`, которая позволяет писать код для отображения в виде `HTML` тэгов, хотя, по сути, это не тэги, а обычные объекты `JavaScript`.

Пример:
```jsx
<div style={{ width: '500px' }}>
    <span className="class">Какой то тект</span>
    <MyCustomAlert title="Этот текст будет показан как бы вверху уведомления">
        Текст внутри нашего компонента
    </MyCustomAlert>
</div>
```

### Структура компонента React
У каждого компонента в `React` есть так называемые `props` ("пропсы", как многие их называют на русском). При каждом измении любого свойства из `props`, компонент изменяет свое отображение и поведение.

Компоненты бывают 2 типов: функциональные и реализованные с помощью класса (считаются основными). В рамках данного воркшопа мы будем рассматривать функциональные компоненты, потому что их легче и быстрее понять.

Функциональный компонент - это функция `JavaScript`, которая принимает несколько параметров и возвращает объекты `JSX`. Далее под словом компонент будет пониматься именно функциональный компонент.

## React Native
Библиотека `React Native` тоже была создана кампанией Facebook и позволяет не только строить отображение приложения, но и использовать "фишки" мобильных устройств, такие как постоянное хранилище, работу в выключенном состоянии и даже push-уведомления.

## Запуск приложения
Для запуска приложения на мобилке, его необходимо собрать. К сожалению, этот процесс не быстрый и для разработки не подходит.

Для `React Native` была разработана библиотека компонентов `Expo`, которая так же позволяет запускать приложение на телефоне без этапа сборки. Мы будем использовать `Expo` для запуска и просмотром изменений.

>> Ваше мобильное устройство должно находиться в одной сети с вашим компьютером.

1. Скачайте приложение `Expo` на свое мобильное устройство.
    - Google play ![QR Expo Client on Google Play](https://github.com/dmitryrykov-epam/react-native-student-schedule-learn/tree/master/lessons/assets/g-play-expo.png)
    - AppStore ![QR Expo Client on AppStore](https://github.com/dmitryrykov-epam/react-native-student-schedule-learn/tree/master/lessons/assets/i-store-expo.png)
2. Запустите приложение на мобильном устройстве.
3. На компьютере в терминале/консоли перейдите в корневую директорию проекта и запустите команду `npm start`
4. Подождите, пока в выводе терминала/консоли не появится QR-код
>> Если у вас терминал/консоль имеют белый задний фон, то вы не сможете увидеть QR-код, так как он рисуется белыми символами. Используйте другую утилиту или измените цвет фона.
5. Просканируйте этот QR-код с помощью приложения `Expo Client` со своего мобильного устройства.

Теперь все изменения программы вы будете видеть на своем мобильном устройсвте "в живую".

## Руководство
Откройте файл `lessons/component.md` или перейдтие [по ссылке](https://github.com/dmitryrykov-epam/react-native-student-schedule-learn/tree/master/lessons/component.md). Там вы увидите описание дальнейшего плана работы.
