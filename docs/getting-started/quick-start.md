# Быстрый старт

Этот раздел поможет вам быстро начать работу с Oasis 3D.

## Первые шаги

### 1. Инициализация проекта

```bash
3doasis init my-project
cd my-project
```

### 2. Базовая конфигурация

Создайте файл `config.yaml`:

```yaml
project:
  name: "My Project"
  version: "1.0.0"

settings:
  debug: false
  verbose: true
```

### 3. Запуск

```bash
3doasis run
```

## Пример использования

Вот простой пример кода:

```python
import 3doasis

# Создание экземпляра
app = 3doasis.Application()

# Настройка
app.configure({
    'setting1': 'value1',
    'setting2': 'value2'
})

# Запуск
app.run()
```

## Что дальше?

- Изучите [Configuration](configuration.md) для детальной настройки
- Посмотрите [User Guide](../user-guide/overview.md) для подробной информации
- Изучите [Examples](../user-guide/examples.md) для большего количества примеров