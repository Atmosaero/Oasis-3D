# Настройка окружения для разработки

Этот раздел описывает, как настроить окружение для разработки Oasis 3D.

## Требования

Для разработки вам понадобятся:

- Python 3.8+
- Git
- Ваш любимый редактор кода (VS Code, PyCharm, и т.д.)

## Клонирование репозитория

```bash
git clone https://github.com/Atmosaero/Oasis-3D.git
cd Oasis-3D
```

## Создание виртуального окружения

### Windows

```powershell
python -m venv venv
.\venv\Scripts\activate
```

### Linux/Mac

```bash
python3 -m venv venv
source venv/bin/activate
```

## Установка зависимостей

```bash
pip install -r requirements.txt
pip install -r requirements-dev.txt  # Если есть
```

## Установка в режиме разработки

```bash
pip install -e .
```

## Запуск тестов

```bash
pytest
```

## Запуск линтера

```bash
flake8 .
black --check .
```

## Следующие шаги

- Прочитайте [Contributing Guide](contributing.md)
- Изучите [Guidelines](guidelines.md)