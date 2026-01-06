# Базовое использование

Этот туториал поможет вам начать работу с Oasis 3D.

## Шаг 1: Установка

См. [Installation Guide](../getting-started/installation.md)

## Шаг 2: Создание проекта

```bash
3doasis init my-first-project
cd my-first-project
```

## Шаг 3: Базовая настройка

Создайте файл `config.yaml`:

```yaml
project:
  name: "My First Project"
  version: "0.1.0"
```

## Шаг 4: Первый код

Создайте файл `main.py`:

```python
import 3doasis

def main():
    app = 3doasis.Application()
    app.configure({
        'debug': True
    })
    app.run()

if __name__ == '__main__':
    main()
```

## Шаг 5: Запуск

```bash
python main.py
```

## Что дальше?

- Изучите [Advanced Topics](advanced-topics.md)
- Посмотрите [Examples](../user-guide/examples.md)
- Прочитайте [API Reference](../api/overview.md)