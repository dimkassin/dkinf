## Стиль коммитов

Мы используем [Conventional Commits](https://www.conventionalcommits.org/) для форматирования наших сообщений коммитов. При коммите, сообщения будут проверяться на соответствие этому стандарту с помощью [commitlint](https://commitlint.js.org/).

Сообщения коммитов в формате Conventional Commits следуют определенной структуре. Вот как выглядит общий формат:
  
```sh
<type>: <description>npm install husky --save-dev
```
type - это тип изменения, которое вы внесли в коммит. Это может быть feat (для новой функциональности),  
fix (для исправления ошибок), docs (для изменений в документации), style (для кода, который не влияет на логику работы, например,  форматирование),  
refactor (для рефакторинга кода), test (для добавления отсутствующих тестов или исправления существующих),  
chore (для обновления сборщика, добавления библиотек и т.д.).  
  
description - это короткое описание того, что делает коммит.  
  
### Пример

```sh
git commit -m "feat: add new feature"
```

В этом репозитории находится пример приложения с тестами:

- [e2e тесты](e2e/example.spec.ts)
- [unit тесты](src/example.test.tsx)

Для запуска примеров необходимо установить [NodeJS](https://nodejs.org/en/download/) 16 или выше.

Как запустить:

```sh
# установить зависимости
npm ci

# запустить приложение
npm start
```

Как запустить e2e тесты:

```sh
# скачать браузеры
npx playwright install

# запустить тесты
npm run e2e
```

Как запустить модульные тесты:

```sh
npm test
```