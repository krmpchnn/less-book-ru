# Где публикуется переводимая книга?

https://krmpchnn.github.io/less-book-ru/ - это адрес, куда инкрементально выкладывается перевод книги с каждым изменением кода.

# Как участвовать в проекте?

1. Вы понимаете Scrum и LeSS (в идеале, вы читали эту книгу и другие две книги в оригинале), были на тренингах.

1. Вы добавились в [Trello доску](https://trello.com/invite/b/0E823LS1/b26d345a86962146498c91207612074c/less-book-ru). Любая работа, которую вы делаете, должна быть отражена на доске. Мы помним, что важно минимизировать WIP, и, так как книга публикуется в сеть инкрементально, лучше иметь первые статьи готовыми, чем много полуготовых.

1. Вы ознакомились с [терминологией](https://github.com/krmpchnn/less-book-ru/blob/gh-pages/.dictionary). В случае корректировок - вы можете предложить изменение в этом файле.

1. Вы понимаете, как работать с GitHub или Git. Вы можете использовать любой текстовый редактор или IDE. Включая просто редактирование в браузере (пример ниже).

1. Вы понимаете, как писать в [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

1. У вас открыта оригинальная [книга на английском](https://github.com/krmpchnn/less-book-ru/blob/gh-pages/assets/pdf/less-book-en.pdf).

1. Вы выбрали главу для редактирования как [файл chapterN.md](https://github.com/krmpchnn/less-book-ru) или же создали пустой файл главы chapterN.md и наполняете его содержимым из [PDF исходник с некачественным переводом](https://github.com/krmpchnn/less-book-ru/blob/gh-pages/assets/pdf/less-book-ru.pdf).

1. Наша задача - выпустить онлайн книгу, которая по своей вёрстке близка к оригинальному PDF, так что нам важны

*курсивы* в тексте

````
делаются так: 
*курсивы* в тексте
````

> цитаты и выделения

````
делаются так: 
> цитаты и выделения
````

```` вставки вроде этой ````

````
делаются так: 
```` вставки вроде этой ````
````

картинки, который вы добавляете в папку [assets/images](https://github.com/krmpchnn/less-book-ru/tree/gh-pages/assets/images), беря их [с сайта less.works](https://less.works/resources/graphics/book-images.html)

````
картинки вставлюятся так: 
![название картинки](/assets/images/filename.png)

````

Ниже вы найдёте детальное руководство по Markdown.

# Как работать прямо в GitHub (для непрограммистов)

Вы можете использовать файл [test.md](https://github.com/krmpchnn/less-book-ru/blob/gh-pages/test.md) для тестирования работы с GitHub, не боясь что-то сломать.

## Открываем главу на редактирование (и да! меняем статус в Trello параллельно на "In Work")

![открываем редактирование](/assets/images/howto-edit.png)

## Редактируем как Markdown текст

![редактируем](/assets/images/howto-markdown.png)

## Пишем комментарий и коммитим изменение в свою временную ветку

![коммитим](/assets/images/howto-commit.png)

### Дожидаемся сборки

![ждём](/assets/images/howto-wait-build.png)

## Создаём pull request, чтобы кто-то проверил и склеил изменения

![коммитим](/assets/images/howto-pr.png)

## Ждём, пока кто-то проверит  наши изменения (и да! меняем статус в Trello параллельно на "Ready for Review")

![делаем pr](/assets/images/howto-wait-build.png)

## Кто-то находит ваш pull request

![находим pr](/assets/images/howto-see-pr.png)

## И запускает ревью

![запускаем ревью](/assets/images/howto-pr-review.png)

## Принимает ваши изменения

![запускаем ревью](/assets/images/howto-pr-approve.png)

## Убеждаемся, что мы понимаем ошибки, если они есть

![смотрим на ошибки](/assets/images/howto-checks.png)

![понимаем проблему](/assets/images/howto-read-checks.png)

# Для программистов (для тех, кто будет переводить в среде разработки)

В проекте существует автоматическая проверка орфографии и структуры статей на русском языке, её конфигурация находится в папке .github (технология [Github Actions](https://github.com/krmpchnn/less-book-ru/actions)).

1. После каждого пуша новой порции перевода запускается проверка орфографии, и вы увидите красный крестик рядом со своим коммитом, если в тексте будут ошибки
1. Вы можете локально проверить орфографию и структуру MD-файлов без отправки изменений на сервер. Для этого необходимо установить [Node.JS+NPM v10+](https://nodejs.org/ru/download/), следуя инструкции по вашей операционной системе
1. После установки Node.JS+NPM достаточно в консоли в корне репозитория запустить команду для проверки структуры ```npx markdownlint-cli **/*.md```. Если добавить ключ ```--fix```, то линтер поправить все ошибки сам.
1. Если вы считаете, что проверка сработала ошибочно, то можете отредактировать .markdownlintrc. Подробнее о настройке [markdownlint](https://github.com/DavidAnson/markdownlint#optionsconfig).
1. После установки Node.JS+NPM достаточно в консоли в корне репозитория запустить команду для проверки орфографии```npx yaspeller -l ru .```.
1. Если вы считаете, что проверка сработала ошибочно, то можете добавить ваши исключения в файл .yaspellerrc в алфавитном порядке. Подробнее о [yaspeller](https://github.com/hcodes/yaspeller).

# Самое важное в Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

> Quote or a blockquote
> This is again a quote.

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

Читайте больше о формате [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).
