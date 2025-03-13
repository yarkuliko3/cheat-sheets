# Шпаргалка по Git

## Основные команды

### Инициализация репозитория
```bash
git init
```

### Клонирование репозитория
```bash
git clone <url>
```

### Проверка статуса
```bash
git status
```

### Добавление файлов в индекс
```bash
git add <file>
git add .  # Добавить все изменения
```

### Коммит изменений
```bash
git commit -m "Сообщение коммита"
```

### Просмотр истории коммитов
```bash
git log
git log --oneline  # Краткий вывод
```

### Просмотр изменений
```bash
git diff
git diff --staged  # Просмотр изменений в индексе
```

## Ветки

### Создание новой ветки
```bash
git branch <branch_name>
```

### Переключение на ветку
```bash
git checkout <branch_name>
git switch <branch_name>  # Альтернатива
```

### Создание и переключение на новую ветку
```bash
git checkout -b <branch_name>
git switch -c <branch_name>  # Альтернатива
```

### Удаление ветки
```bash
git branch -d <branch_name>
```

### Слияние веток
```bash
git merge <branch_name>
```

### Перебазирование
```bash
git rebase <branch_name>
```

## Удаленные репозитории

### Добавление удаленного репозитория
```bash
git remote add origin <url>
```

### Просмотр удаленных репозиториев
```bash
git remote -v
```

### Отправка изменений на удаленный репозиторий
```bash
git push origin <branch_name>
```

### Получение изменений с удаленного репозитория
```bash
git pull origin <branch_name>
```

### Клонирование удаленного репозитория
```bash
git clone <url>
```

## Отмена изменений

### Отмена изменений в рабочей директории
```bash
git checkout -- <file>
```

### Отмена индексации файла
```bash
git reset <file>
```

### Отмена последнего коммита
```bash
git reset --soft HEAD~1
```

### Отмена последнего коммита и всех изменений
```bash
git reset --hard HEAD~1
```

## Теги

### Создание тега
```bash
git tag <tag_name>
```

### Создание аннотированного тега
```bash
git tag -a <tag_name> -m "Сообщение тега"
```

### Просмотр тегов
```bash
git tag
```

### Отправка тегов на удаленный репозиторий
```bash
git push origin --tags
```

## Прочее

### Просмотр изменений в конкретном коммите
```bash
git show <commit_hash>
```

### Просмотр изменений между двумя коммитами
```bash
git diff <commit_hash_1> <commit_hash_2>
```

### Сохранение временных изменений (stash)
```bash
git stash
git stash pop  # Применить изменения и удалить из stash
```

### Просмотр списка stash
```bash
git stash list
```

### Очистка рабочей директории
```bash
git clean -fd
```

## Полезные алиасы

### Добавление алиасов в конфигурацию Git
```bash
git config --global alias.co checkout
git config --global alias.br branch
git config --global alias.ci commit
git config --global alias.st status
```

Теперь вы можете использовать `git co` вместо `git checkout`, `git br` вместо `git branch` и т.д.
```
