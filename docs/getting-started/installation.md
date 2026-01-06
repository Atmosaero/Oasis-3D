# Установка

В этом разделе описано, как установить и настроить Oasis 3D.

## Требования

Перед установкой убедитесь, что у вас установлены следующие компоненты:

- Python 3.8 или выше
- pip (менеджер пакетов Python)
- Git

## Установка

### Способ 1: Через pip

```bash
pip install 3doasis
```

### Способ 2: Из исходников

```bash
git clone https://github.com/your-username/Oasis 3D.git
cd Oasis 3D
pip install -e .
```

### Способ 3: Через conda

```bash
conda install -c conda-forge 3doasis
```

## Проверка установки

После установки проверьте, что всё работает корректно:

```bash
3doasis --version
```

Вы должны увидеть номер версии, например: `Oasis 3D 1.0.0`

## Следующие шаги

После успешной установки перейдите к разделу [Quick Start](quick-start.md) для начала работы.