# proyecto_mini_turtle

Mini librería para dibujar trazos en consola simulando una "mini tortuga".

## Descripción
Este proyecto proporciona funciones sencillas para mover una tortuga en una cuadrícula de texto:
- `adelante(pasos)` dibuja una línea horizontal hacia la derecha.
- `abajo(pasos)` dibuja una columna vertical hacia abajo.
- `reiniciar()` vuelve a la posición inicial (0,0).

Las funciones están disponibles desde el paquete `mini_turtle`.

## Instalación
No hay dependencias externas. Simplemente coloca el paquete en tu proyecto o ejecuta los scripts directamente.

## Uso básico
Ejemplo mínimo (ver [main.py](main.py)):

```python
from mini_turtle import adelante, abajo, reiniciar

reiniciar()
adelante(7)
abajo(3)
```

Salida esperada en consola (ejemplo):
```
------->        # línea horizontal de 7 pasos
       |
       |
       |
       V
```

Ejecuta el script principal:
```sh
python main.py
```

## API
- [`mini_turtle.adelante`](mini_turtle/__init__.py) — dibuja `-` repetidos y avanza la posición X.
- [`mini_turtle.abajo`](mini_turtle/__init__.py) — dibuja `|` en la columna actual y marca con `V` al final; avanza la posición Y.
- [`mini_turtle.reiniciar`](mini_turtle/__init__.py) — resetea las posiciones X e Y a 0.

Implementación principal: [mini_turtle/draewer_logic.py](mini_turtle/draewer_logic.py)

## Ejemplos adicionales
Puedes combinar llamadas para crear figuras simples. Consulta [main.py](main.py) para ejemplos de uso.

## Licencia
Este proyecto está bajo la licencia MIT. Consulta [LICENSE](LICENSE).