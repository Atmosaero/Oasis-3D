# API Reference - Components

Документация компонентов Oasis 3D API.

## ComponentBase

Базовый класс для всех компонентов.

```python
class ComponentBase:
    """Базовый компонент системы."""
    
    def __init__(self, config: dict = None):
        """
        Инициализация компонента.
        
        Args:
            config: Конфигурация компонента
        """
        pass
    
    def initialize(self):
        """Инициализация компонента."""
        pass
    
    def cleanup(self):
        """Очистка ресурсов компонента."""
        pass
```

## Component1

Описание компонента 1.

```python
class Component1(ComponentBase):
    """Компонент для [описание назначения]."""
    
    def method1(self, param: str) -> str:
        """
        Метод компонента.
        
        Args:
            param: Параметр метода
            
        Returns:
            Результат выполнения
        """
        pass
```

## Component2

Описание компонента 2.

```python
class Component2(ComponentBase):
    """Компонент для [описание назначения]."""
    
    def method1(self, param: int) -> bool:
        """
        Метод компонента.
        
        Args:
            param: Параметр метода
            
        Returns:
            Результат выполнения
        """
        pass
```

## Использование компонентов

```python
from 3doasis.components import Component1, Component2

# Создание компонентов
comp1 = Component1(config={'setting': 'value'})
comp2 = Component2()

# Инициализация
comp1.initialize()
comp2.initialize()

# Использование
result = comp1.method1('test')
success = comp2.method1(42)

# Очистка
comp1.cleanup()
comp2.cleanup()
```