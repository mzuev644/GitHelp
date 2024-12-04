# Шапргалка по Git

<br />

## Подготовка репозитория

#### Установка имени и электронной почты
```bash
git config --global user.name "Your Name"
git config --global user.email "your_email@whatever.com"
```
#### Создание репозитория
```bash
git init
```

<br />

## Индексация и коммиты

#### Проверка состояния репозитория
```bash
git status
```

#### Индексация
```bash
git add <имя_файла>
```
Индексировать весь репозиторий: `--all`

#### Коммит
```bash
git commit -m "Комментарий"
```

#### История коммитов
```bash
git log
```
Однострочная история: `--pretty=oneline`

[Другие опции](https://git-scm.com/docs/git-log)

<br />

## Работа с ветками

#### Создание ветки
```bash
git switch -c
```

#### Переключение между ветками
```bash
git switch <имя_ветки>
```
Предыдущий коммит: `<хеш_коммита>^`

#### Создание тегов
```bash
git tag <имя_тега>
```

#### Отмена изменений в рабочем каталоге (файл изменен, но не проиндексирован)
```bash
git checkout <имя_файла>
```

#### Отмена проиндексированного файла
```bash
git reset HEAD <имя_файла>
git checkout <имя_файла>
```

#### Отмена коммита
```bash
git revert HEAD
```

