# Как контрибьютить в проект?

1. Вы понимаете Scrum и LeSS (в идеале, вы читали эту книгу и другие две книги в оригинале), были на тренингах.

1. Вы добавились в [Trello доску](https://trello.com/invite/b/0E823LS1/b26d345a86962146498c91207612074c/less-book-ru). Любая работа, которую вы делаете, должна быть отражена на доске. Мы помним, что важно минимизировать WIP, и, так как книга публикуется в сеть инкрементально, лучше иметь первые статьи готовыми, чем много полуготовых.

1. Вы ознакомились с [терминологией](https://github.com/krmpchnn/less-book-ru/blob/gh-pages/.dictionary). В случае корректировок - вы можете предложить изменение в этом файле.

1. Вы понимаете, как работать с GitHub или Git. Вы можете использовать любой текстовый редактор или IDE. Включая просто редактирование в браузере (пример ниже).

1. Вы понимаете, как писать в [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

1. У вас открыта оригинальная [книга на английском](https://github.com/krmpchnn/less-book-ru/blob/gh-pages/assets/pdf/less-book-en.pdf).

1. Вы выбрали главу для редактирования как [файл chapterN.md](https://github.com/krmpchnn/less-book-ru) или же создали пустой файл главы chapterN.md и наполяете его содержимым из [PDF исходник с некачественным переводом](https://github.com/krmpchnn/less-book-ru/blob/gh-pages/assets/pdf/less-book-ru.pdf).

1. Наша задача - выпустить онлайн книгу, которая по своей вёрстке близка к оригинальному PDF, так что нам важны
 - *курсивы* в тексте
 - > цитаты и выделения
 - ``` вставки вроде этой ```
 - картинки, который вы добавляте в папку [assets/images](https://github.com/krmpchnn/less-book-ru/tree/gh-pages/assets/images), беря их [с сайта less.works](https://less.works/resources/graphics/book-images.html)
 - всяческие ремарки, футноуты и хинты на полях - пишем их прямо в тексте, так как в Markdown нет таких фич.

## Как работать прямо в GitHub (для непрограммистов)

### Открываем главу на редактирование (и да! меняем статус в Trello параллельно на "In Work").

![открываем редактирование](/assets/images/howto-edit.png)

### Редактируем как Markdown текст.

![редактируем](/assets/images/howto-markdown.png)

### Пишем комментарий и коммитим изменение в свою временную ветку.

![коммитим](/assets/images/howto-commit.png)

### Создаём pull request, чтобы кто-то проверил и смержил изменения

![коммитим](/assets/images/howto-pr.png)

### Ждём, пока кто-то поревьювает наши изменения (и да! меняем статус в Trello параллельно на "Ready for Review").

![делаем pr](/assets/images/howto-pr-waiting.png)

### Кто-то находит ваш pull request.

![находим pr](/assets/images/howto-see-pr.png)

### И запускает ревью.

![запускаем ревью](/assets/images/howto-pr-review.png)

### Принимает ваши изменения.

![запускаем ревью](/assets/images/howto-pr-approve.png)

### Убеждаемся, что мы понимаем ошибки, если они есть.

![смотрим на ошибки](/assets/images/howto-checks.png)

![понимаем проблему](/assets/images/howto-read-checks.png)

## Самое важное в Markdown

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

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

