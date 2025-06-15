# 🚀 Настройка GitHub репозитория

## Шаг 1: Создайте репозиторий на GitHub

1. Перейдите на https://github.com
2. Нажмите "New repository" (зеленая кнопка)
3. Название: `exam-ticket-generator` 
4. Описание: `🎓 Universal Exam Ticket Generator - Python script for creating exam tickets from Word documents (Uzbek/Russian)`
5. Выберите "Public" (для портфолио)
6. НЕ добавляйте README, .gitignore, license (они уже есть)
7. Нажмите "Create repository"

## Шаг 2: Подключите локальный репозиторий

Выполните команды в терминале в папке `/Users/temur/Desktop/Claude`:

```bash
# Добавить удаленный репозиторий (замените USERNAME на ваш GitHub username)
git remote add origin https://github.com/USERNAME/exam-ticket-generator.git

# Переименовать ветку в main (современный стандарт)
git branch -M main

# Запушить код на GitHub
git push -u origin main
```

## Пример команд для вашего случая:

```bash
git remote add origin https://github.com/TemurTurayev/exam-ticket-generator.git
git branch -M main  
git push -u origin main
```

## Шаг 3: Проверьте результат

После выполнения команд:
1. Обновите страницу репозитория на GitHub
2. Убедитесь, что все файлы загружены
3. README.md должен отображаться как главная страница

## Шаг 4: Добавьте темы (topics) для SEO

На странице репозитория:
1. Нажмите на шестеренку рядом с "About"
2. Добавьте темы: `python`, `exam`, `education`, `uzbek`, `russian`, `medical-education`, `tashpmi`, `word-processing`, `automation`

## Шаг 5: Поделитесь ссылкой

Ваш репозиторий будет доступен по адресу:
`https://github.com/TemurTurayev/exam-ticket-generator`

## 🔧 Если возникают проблемы:

### Проблема: "Permission denied"
```bash
# Используйте personal access token вместо пароля
# Настройте в Settings > Developer settings > Personal access tokens
```

### Проблема: "Repository not found"
```bash
# Проверьте правильность URL
git remote -v  # показать текущие remotes
git remote set-url origin CORRECT_URL  # исправить URL
```

### Проблема: "Updates were rejected"  
```bash
# Если удаленный репозиторий не пустой
git pull origin main --allow-unrelated-histories
git push origin main
```

## 🎉 Готово!

После успешного пуша ваш проект будет:
- ✅ Доступен в интернете
- ✅ Хорош для портфолио
- ✅ Иметь красивый README
- ✅ Готов для других разработчиков
- ✅ Профессионально оформлен