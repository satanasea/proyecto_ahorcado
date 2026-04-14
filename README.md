# 🎯 Juego del Ahorcado en Python

Proyecto desarrollado para el curso **Programación para la Ciencia e Ingeniería**  
Universidad Mariano Gálvez de Guatemala — Campus Antigua

---

## 📋 Descripción

Implementación del clásico juego del **Ahorcado** en Python. El programa selecciona aleatoriamente una palabra oculta relacionada con ingeniería y computación. El jugador debe adivinarla letra por letra antes de agotar los **6 intentos** disponibles.

---

## 🚀 Cómo ejecutar

### Requisitos
- Python 3.x instalado

### Pasos
```bash
# Clona el repositorio
git clone https://github.com/satanasea/proyecto_ahorcado.git

# Entra a la carpeta
cd ahorcado-python

# Ejecuta el juego
python ahocado_juego.py
```

---

## 🎮 Cómo se juega

1. El programa muestra la palabra oculta como guiones: `_ _ _ _ _ _`
2. Ingresa una letra por turno
3. Si la letra **está** en la palabra → se revela en su posición
4. Si la letra **no está** → se descuenta un intento
5. Ganas al completar la palabra / Pierdes al llegar a 0 intentos

**Ejemplo de ejecución:**
```
Palabra: _ _ _ _ _ _ _ _ _
Intentos restantes: 6
Ingresa una letra: p

Bien hecho! La 'p' es correcta.

Palabra: p _ _ _ _ _ _ _ _
Intentos restantes: 6
Ingresa una letra: z

Lo siento, la 'z' no esta en la palabra.

Palabra: p _ _ _ _ _ _ _ _
Intentos restantes: 5
```

---

## 🏗️ Estructura del código

```
ahocado_juego.py
│
├── CONFIGURACION          # Tupla con constantes del juego
├── seleccionar_palabra()  # Elige palabra aleatoria del banco
├── mostrar_tablero()      # Muestra estado actual del juego
├── validar_letra()        # Valida entrada del usuario
└── jugar()                # Función principal — controla el flujo
```

---

## 🧩 Conceptos aplicados

| Estructura | Uso en el programa |
|---|---|
| `tuple` | `CONFIGURACION` — almacena constantes inmutables |
| `list` | Banco de palabras, palabra oculta, historial de letras |
| `while` | Ciclo principal del juego |
| `for` + `range()` | Actualizar posiciones al acertar una letra |
| `if / else` | Validar entrada y determinar resultado final |
| `f-strings` | Mensajes dinámicos en consola |
| `random.choice()` | Selección aleatoria de palabra |
| `-=` | Operador de asignación compuesta para descontar intentos |

---

## 📁 Archivos

```
ahorcado-python/
├── ahocado_juego.py   # Código fuente del juego
└── README.md          # Este archivo
```

---

## 🎬 Video explicativo

▶️ [Ver en YouTube](https://youtu.be/J6xTZQ59J_0?si=FZvxxvD3wOk_o607)

El video cubre el funcionamiento del código y explica el uso de cada estructura de programación.

---

## 👤 Autor

**Eduardo Alejandro García González**  
Carnet: 1010-26-22472  
Ingeniería Civil — Universidad Mariano Gálvez de Guatemala  

---

## 📌 Nota

Proyecto académico desarrollado como práctica del segundo parcial, 13 de abril de 2026.
