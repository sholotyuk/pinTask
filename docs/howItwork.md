# pinTask

## Додаток для простого списку справ
Це дозволяє користувачам створювати нові списки справ і додавати до них завдання.

## Упровадження
*Vue* розроблений для поступового впровадження у проєкт. Це означає можливість його використання у кілька способів у залежності від вимог:
- Імпортування на сторінку як CDN-пакет (Content Delivey Network — мережа розповсюдження даних). Це зручно для створення прототипів або навчання. Потрібно просто додати один рядок у тег ```head```: 
```
<script src="https://unpkg.com/vue@next"></script>
```
  >Це забезпечить використання останньої версії Vue.
- Установлення через npm. Рекомендований спосіб для створення великих проєктів. Він повністю узгоджений із зв'язниками модулів, такими як [Webpack](https://webpack.js.org/) та [Rollup](https://rollupjs.org/guide/en/). Для встановлення останньої версії Vue, потрібно виконати команду:
```
npm install vue@next
```
- Використання Vue CLI (Command-Line Interface — інтерфейс через командний рядок). Є розширенням попереднього пункту, яке дозволяє швидко створювати SPA. Він має налаштування зібрання проєкту для сучасного робочого процесу. Можна швидко бачити результат разом з hot reload (миттєве відображення змін без перезавантаження сторінки), lint on save (виявлення вад коду з його збереженням) та готовими збірками проєкту. Для встановлення останньої версії Vue CLI, з правами адміністратора потрібно виконати команду:
```
npm install -g @vue/cli
```
- Проєкт *Vue* також можна швидко налаштувати за допомогою *Vite*, виконавши наступні команди в вашому терміналі:
```
npm init @vitejs/app <project-name>
cd <project-name>
npm install
npm run dev
```
## Структура проєкта та запуск додатка
Весь код знаходиться у папці ```src```, зміст якої:
- папка assets зберігає допоміжні файли (наприклад, зображення)
- папка ```components``` зберігає компоненти, з яких складається застосунок (в нашому випадку - це ```TaskCard.vue``` та ```TaskInput.vue```)
- файл ```App.vue``` — головний файл застосунку, який є компонентом за структурою
- файл ```main.js``` додає компонент ```App``` у відповідне місце в документі-шаблоні ```index.html```, який знаходиться у папці ```public``` поруч із папкою ```assets``` (це його єдина функція)

Для зібрання проєкту та запуску сервера, у його папці потрібно виконати команду:
```
npm run dev
```

Перейти на сторінку застосунку можна за адресою:
```
> paintask@0.0.0 dev C:\Users\HP\pinTask
> vite


  vite v2.3.3 dev server running at:

  > Local: http://localhost:3000/
  > Network: use `--host` to expose

  ready in 470ms.

```
## Скріншоти
![alt text](images/interface1.png)
![alt text](images/interface2.png)
![alt text](images/interface3.png)
