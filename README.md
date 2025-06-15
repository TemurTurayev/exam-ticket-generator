# 🎓 Exam Ticket Generator / Генератор Экзаменационных Билетов

[![Python](https://img.shields.io/badge/Python-3.6+-blue.svg)](https://python.org)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/Platform-Cross--Platform-lightgrey.svg)]()

## 🌟 Overview / Обзор

**English:** Universal Python script for generating exam tickets from Word documents. Supports Uzbek and Russian languages, automatically extracts questions from tables and creates beautifully formatted exam tickets.

**Русский:** Универсальный Python-скрипт для создания экзаменационных билетов из Word документов. Поддерживает узбекский и русский языки, автоматически извлекает вопросы из таблиц и создает красиво отформатированные билеты.

## ✨ Features / Возможности

- 📋 **Extract questions from Word tables** / Извлечение вопросов из Word таблиц
- 🌍 **Multi-language support** (Uzbek, Russian) / Поддержка многих языков
- 🔄 **Automatic question repetition** when needed / Автоматическое повторение вопросов
- 🎲 **Random question distribution** / Случайное распределение вопросов  
- 🎨 **Beautiful formatting** / Красивое форматирование
- 📝 **Question numbering** for easy answer lookup / Нумерация для поиска ответов
- 💻 **Command line & interactive modes** / Командная строка и интерактивный режим

## 🚀 Quick Start / Быстрый старт

### Installation / Установка

```bash
# Clone repository / Клонировать репозиторий
git clone https://github.com/TemurTurayev/exam-ticket-generator.git
cd exam-ticket-generator

# Install dependencies / Установить зависимости
pip install python-docx
```

### Basic Usage / Базовое использование

```bash
# Interactive mode / Интерактивный режим
python универсальный_генератор_билетов.py

# Command line / Командная строка
python универсальный_генератор_билетов.py --language uzbek --tickets 360
python универсальный_генератор_билетов.py --language russian --tickets 160
```

## 📁 File Structure / Структура файлов

```
project/
├── универсальный_генератор_билетов.py  # Main script / Основной скрипт
├── ИНСТРУКЦИЯ_ПО_ИСПОЛЬЗОВАНИЮ.md      # Detailed guide / Подробная инструкция
├── README.md                            # This file / Этот файл
├── requirements.txt                     # Dependencies / Зависимости
└── examples/                           # Example files / Примеры файлов
    ├── Адабиёт ўзбек савол.docx        # Uzbek literature questions
    ├── Тарбия ўзбек савол.docx         # Uzbek ethics questions  
    ├── Тарих ўзбек савол.docx          # Uzbek history questions
    ├── Адабиёт рус савол.docx          # Russian literature questions
    ├── Тарбия рус савол.docx           # Russian ethics questions
    └── Тарих рус савол.docx            # Russian history questions
```

## 📊 Input Format / Формат входных данных

Questions should be in Word tables with this structure:
Вопросы должны быть в таблицах Word со следующей структурой:

| № | Question / Вопрос |
|---|-------------------|
| 1 | First question text / Текст первого вопроса |
| 2 | Second question text / Текст второго вопроса |
| ... | ... |

## 🛠️ Command Line Options / Опции командной строки

| Option | Short | Description | Default |
|--------|-------|-------------|---------|
| `--path` | `-p` | Path to folder with question files | Current folder |
| `--tickets` | `-t` | Number of tickets to generate | 360 |
| `--language` | `-l` | Language (uzbek/russian) | uzbek |
| `--output` | `-o` | Output filename | Auto-generated |
| `--help` | `-h` | Show help message | - |

## 💻 Examples / Примеры

### Generate 360 Uzbek tickets / Создать 360 узбекских билетов:
```bash
python универсальный_генератор_билетов.py -l uzbek -t 360 -p ./questions/
```

### Generate 160 Russian tickets / Создать 160 русских билетов:
```bash
python универсальный_генератор_билетов.py -l russian -t 160 -o "RUSSIAN_TICKETS.docx"
```

### Custom ticket count / Произвольное количество билетов:
```bash
python универсальный_генератор_билетов.py -t 500 -l uzbek
```

## 📋 Output / Результат

The script generates formatted Word documents with exam tickets:
Скрипт создает отформатированные Word документы с билетами:

```
БИЛЕТ № 1

1. ЛИТЕРАТУРА
   Вопрос №15:
   What are the main literary genres?

2. ВОСПИТАНИЕ  
   Вопрос №8:
   What is patriotism?

3. ИСТОРИЯ
   Вопрос №142:
   Tell about Uzbekistan's independence.
```

## 🔧 Requirements / Требования

- Python 3.6+
- python-docx library
- Word documents (.docx format)

## 📚 Documentation / Документация

- [Detailed User Guide / Подробная инструкция](ИНСТРУКЦИЯ_ПО_ИСПОЛЬЗОВАНИЮ.md)
- [API Documentation / API документация](docs/api.md) *(coming soon)*

## 🤝 Contributing / Вклад в проект

Contributions are welcome! / Приветствуются любые вклады!

1. Fork the repository / Сделайте форк репозитория
2. Create feature branch / Создайте ветку для новой функции
3. Make your changes / Внесите изменения
4. Submit pull request / Отправьте pull request

## 🐛 Bug Reports / Сообщения об ошибках

Please report bugs on [GitHub Issues](https://github.com/TemurTurayev/exam-ticket-generator/issues)
Пожалуйста, сообщайте об ошибках в GitHub Issues

## 👨‍💻 Author / Автор

**Temur Turaev** / **Темур Тураев**
- 🎓 5th year medical student at TashPMI / Студент 5-го курса TashPMI
- 🔬 Future pediatrician with bioengineering focus / Будущий педиатр с фокусом на биоинженерию
- 📧 Email: temurturayev7822@gmail.com
- 💬 Telegram: [@Turayev_Temur](https://t.me/Turayev_Temur)
- 💼 LinkedIn: [temur-turaev](https://linkedin.com/in/temur-turaev-389bab27b/)
- 🐙 GitHub: [TemurTurayev](https://github.com/TemurTurayev)

## 🏥 Medical Context / Медицинский контекст

This project was created as part of medical education at Tashkent Pediatric Medical Institute (TashPMI). It demonstrates the intersection of medical studies and programming skills, showcasing how healthcare professionals can leverage technology to improve educational processes.

Этот проект создан в рамках медицинского образования в Ташкентском педиатрическом медицинском институте (TashPMI). Он демонстрирует пересечение медицинских исследований и навыков программирования, показывая, как медицинские работники могут использовать технологии для улучшения образовательных процессов.

## 📄 License / Лицензия

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
Этот проект лицензирован под MIT License - см. файл [LICENSE](LICENSE) для деталей.

## 🌟 Star History

[![Star History Chart](https://api.star-history.com/svg?repos=TemurTurayev/exam-ticket-generator&type=Date)](https://star-history.com/#TemurTurayev/exam-ticket-generator&Date)

---

**Made with ❤️ for TashPMI students** / **Создано с ❤️ для студентов TashPMI**

*If this project helped you, please consider giving it a ⭐!*
*Если этот проект помог вам, пожалуйста, поставьте ⭐!*