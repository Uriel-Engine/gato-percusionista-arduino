# 🐱 Gato Percusionista con Arduino

> Proyecto interactivo estilo **drum pad táctil** usando Arduino, OLED y sensores touch
> Creado por **Uriel Engine**

---

## 📸 Demo

![Demo](https://github.com/Uriel-Engine/gato-percusionista-arduino/blob/main/Gato%20Percusionista.png)

---

## 🧠 Descripción

Este proyecto simula un pequeño **instrumento de percusión interactivo**, donde un gato animado toca tambores en una pantalla OLED dependiendo de la interacción del usuario mediante sensores táctiles.

Cada combinación de toque genera:

* Una **animación diferente**
* Un **sonido único en el buzzer**

---

## 🧰 Materiales

* Arduino UNO
* Pantalla OLED SSD1306 (128x64)
* 2 sensores touch (OKY3420-2)
* 1 buzzer pasivo (OKY3154)
* Cables Dupont

---

## ⚙️ Funcionamiento

El sistema tiene **4 estados principales**:

| Estado    | Acción           | Imagen   | Sonido        |
| --------- | ---------------- | -------- | ------------- |
| Sin toque | Inactivo         | Imagen 1 | 🔇 Sin sonido |
| Touch 1   | Tambor izquierdo | Imagen 2 | 🔉 Grave      |
| Touch 2   | Tambor derecho   | Imagen 3 | 🔊 Agudo      |
| Ambos     | Golpe doble      | Imagen 4 | 🔔 Combinado  |

---

## ⏱️ Características técnicas

* Duración del sonido: **500 ms**
* Tolerancia de doble toque: **80 ms**
* Sistema basado en **máquina de estados**
* Uso de `millis()` (sin `delay()`)
* Bitmaps optimizados en **PROGMEM**

---

## 🔊 Frecuencias del buzzer

```cpp
#define FREQ_LOW 250
#define FREQ_HIGH 500
#define FREQ_COMBO 750
```

---

## 🖥️ Código

El sketch incluye:

* Control de estados
* Lectura de sensores touch
* Renderizado de bitmaps en OLED
* Control preciso del buzzer

Solo necesitas cargar el archivo `.ino` en tu Arduino y listo 🚀

---

## 🎮 Experiencia de uso

Este proyecto funciona como un mini:

🥁 **Drum Pad Digital**
🐱 **Animación interactiva**
🎵 **Instrumento electrónico básico**

Ideal para:

* Proyectos educativos
* Introducción a sistemas embebidos
* Interfaces interactivas

---

## 👨‍💻 Autor

**Uriel Engine**
Proyecto desarrollado como práctica de integración de hardware + animación en sistemas embebidos.

---

## ⭐ Apoya el proyecto

Si te gustó este proyecto:

* Dale ⭐ en GitHub
* Compártelo
* Sígueme para más proyectos de electrónica

---

## 📜 Licencia

Uso libre para fines educativos y personales.
