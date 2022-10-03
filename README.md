# golinks
Assembling Best Practices

### Оформление сообщений log

Если есть возможность обработать ошибку, это стоить делать, т.к. результату нельзя доверять до проверки на наличие ошибок.

К тому же:
- пустой идентификатор темен и полон ужасов;
- непредсказуемое поведение программы (о котором мы не знаем - его нет в логах) расстраивает пользователей и ведет к уменьшению количества $.

Простой пример внутренний пакет логирования, основанный на logrus. Формат вывода:
```bash
{"file":"InfoBotUploader.go:44","function":"main","level":"info","msg":"Bot started","time":"2022-04-20T08:03:53Z"}
```

Статья про логирование [logrus](https://medium.com/maddevs-io/golang-logging-7fdd3da5152f).

P.S. [Поговорки Роба Пайка](https://go-proverbs.github.io/):
- «Ошибки — значения»
- «Не просто проверяйте наличие ошибок, а элегантно их обрабатывайте»
- «Не паникуйте» 

### Codestyle

[Uber guide](https://github.com/sau00/uber-go-guide-ru/blob/master/style.md) - на русском

### Размещение пакетов
[Project standards](https://github.com/golang-standards/project-layout/blob/master/README_ru.md) - на русском

### Безопасная разработка на Go
[Рекомендации OWASP](https://github.com/OWASP/Go-SCP)  

### Линтеры
[Линтеры в Go. Как их готовить.](https://habr.com/ru/post/457970/) - на русском

[Установка](https://golangci-lint.run/usage/install/) golangci-lint и его [настройка](https://github.com/xxpxxxxp/intellij-plugin-golangci-lint) в Goland
