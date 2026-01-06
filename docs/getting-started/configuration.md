# Конфигурация

В этом разделе описаны все параметры конфигурации Oasis 3D.

## Файл конфигурации

Oasis 3D использует файл `config.yaml` для настройки. Файл должен находиться в корне проекта.

## Основные параметры

### Общие настройки

```yaml
project:
  name: "Project Name"
  version: "1.0.0"
  description: "Project description"
```

### Настройки приложения

```yaml
app:
  debug: false
  verbose: true
  log_level: "INFO"
```

### Настройки сервера

```yaml
server:
  host: "localhost"
  port: 8080
  timeout: 30
```

## Переменные окружения

Вы также можете использовать переменные окружения:

```bash
export 3DOASIS_DEBUG=true
export 3DOASIS_LOG_LEVEL=DEBUG
```

## Приоритет настроек

Настройки применяются в следующем порядке (от высшего к низшему):

1. Переменные окружения
2. Файл конфигурации
3. Значения по умолчанию

## Пример полной конфигурации

```yaml
project:
  name: "My Oasis 3D Project"
  version: "1.0.0"

app:
  debug: false
  verbose: true
  log_level: "INFO"

server:
  host: "0.0.0.0"
  port: 8080
  timeout: 30

database:
  type: "sqlite"
  path: "./data.db"

cache:
  enabled: true
  ttl: 3600
```