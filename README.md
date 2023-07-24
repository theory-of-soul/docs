# React JS project
## Подготовка
Настраивается один раз для каждого устройства

### 0. IDE
Надеюсь, что ты используешь какое-нибудь нормальное IDE типа webstorm или vscode 

### 1. Устанавливаем Node.js 
Это необходимо для работы с библиотками, в том числе ReactJS, запуска серверов. https://nodejs.org/en. 
Самый простой способ это сделать скачать на главной установочный файл.

### 2. Устанавливаем Yarn
Необходим для грамотной работы с версиями библиотек. https://yarnpkg.com/getting-started/install. 
В любой библиотеке можно увидеть пример кода: `yarn add lib-name`

### 3. React framework
Самый современный способ использовать React библиотеку сейчас, это использовать её в контексте framework'a. 
Я предлагаю тебе остановиться на `Next.js` - это активно развивающийся full-stack фреймворк. 
Помимо готовой хорошей архитектуры, они так же предоставляют сервера и deploy систему, 
можно спокойно будет сэкономить в первое время на devops-спеицалисте. 

Вот тут можно подробнее посмотреть каждый из тех что популярны сейчас: https://react.dev/learn/start-a-new-react-project

### 3. Установка Next.js
В терминале:
```
npx create-next-app@latest
```
Тебе нужно будет ответить на следующие вопрос вот так: 
```
What is your project named? your-name-app
Would you like to use TypeScript? No
Would you like to use ESLint? Yes
Would you like to use Tailwind CSS? Yes 
Would you like to use `src/` directory? No 
Would you like to use App Router? (recommended) Yes
Would you like to customize the default import alias? No
```
Стили описываем в классах. Это для ускорения разработки и для уменьшения количества строк стилей. 
Подробнее про [Tailwind CSS](https://tailwindcss.com/)

[Документация](https://nextjs.org/docs/getting-started/installation)

### 4. Запускаем проект
```npm run dev``` 

Переходим http://localhost:3000
Проверяем, что изменения `app/page.js` срабатывают


### 5. Архитектура проекта и роутинг 
На выходе получаем готовую, [хорошопродуманную архитектуру](https://nextjs.org/docs/getting-started/project-structure )

Нас сейчас больше всего интересует роутинг, тут всё просто, мы создаем в папке `app` наши пути с помощью папок. Повторем существующий проект. 

Например, `app/dashboard` - будет открываться, как страница http://localhost:3000/dashboard 

Подробнее смотрим [в документации](https://nextjs.org/docs/app/building-your-application/routing#terminology)

### 6. Погружение в React 
Если с React никогда не сталкивался, то советую посмотреть/повторить [основы](https://react.dev/learn) и вот [этот tutorial](https://react.dev/learn/tutorial-tic-tac-toe) там есть использвание [хуков](https://react.dev/learn/tutorial-tic-tac-toe). 

### 7. Библиотеки, которые тебе пригодятся
Библиотек огромное количество, я для тебя подобрала подходящие на мой взгляд, но это при поверхностном просмотре твоего проекта, где-то может и не хватать функицонала, тогда нужно будет менять её - можно будет спросить меня, либо следующий универсальный совет: 

Самостоятельный выбор. Советую смотреть на её поддержку: когда её в последний раз обновляли, сколько там issues, forks и звёзд.

1) Авторизация пользователя, в том числе google/facebook и тд - https://next-auth.js.org/ 
2) Для таблиц есть супер гибкая библиотека, сразу советую смотреть/копировать подходящие тебе примеры, потому что там очень большая документаци, она может отпугнуть - https://tanstack.com/  
3) Для твоих графиков подойдет вот эта библиотека, она легковестная на svg - https://github.com/recharts/recharts
4) Для форм есть официальные рекмендации от next.js, можно тут посмотреть - https://nextjs.org/docs/pages/building-your-application/data-fetching/building-forms
5) Для работы с датами и выбором промежутков может подойти вот эта связка - [react-day-picker](https://react-day-picker.js.org/) и [date-fns](https://date-fns.org/) 

Вот этого всего на данный момент хватит для проекта. 


