# 👾 Pac-Man JS

<div align="center">

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Canvas](https://img.shields.io/badge/Canvas_2D-0099CC?style=for-the-badge)
![Sin dependencias](https://img.shields.io/badge/Sin%20dependencias-3fb950?style=for-the-badge)
![License](https://img.shields.io/badge/Licencia-MIT-yellow?style=for-the-badge)

**Recreación del clásico Pac-Man con IA de fantasmas, power-ups y laberinto completo.**  
Construido desde cero en HTML5 Canvas — sin librerías, sin instalación.

**[▶ Ver demo en vivo](https://suarezsh.github.io/pacman-js)**

</div>

---

## 🎯 ¿Qué es esto?

Una recreación fiel del arcade clásico de 1980 con los 4 fantasmas originales, cada uno con su propia inteligencia artificial, laberinto completo con 176 puntos, poder-ups y sistema de niveles.

---

## ✨ Características

- 🗺️ **Laberinto completo** — 21×23 celdas con túneles laterales y casa de fantasmas
- 👾 **4 fantasmas con IA** — cada uno con personalidad y estrategia distintas
- ⚡ **Power-ups** — 4 power pellets que ponen a los fantasmas en modo asustado
- 💀 **Animación de muerte** — Pac-Man gira y se colapsa al morir
- ⏸️ **Pausa / Reanudar** — con `P` o el botón
- 🎵 **Sonido procedural** — Web Audio API sin archivos externos
- 📱 **Touch** — swipe para cambiar dirección en móvil
- 🔢 **Niveles** — velocidad aumenta con cada nivel completado

---

## 👻 IA de los Fantasmas

| Fantasma | Color | Estrategia |
|---|---|---|
| **Blinky** | 🔴 Rojo | Persigue directamente a Pac-Man |
| **Pinky** | 🩷 Rosa | Se adelanta 4 celdas en la dirección de Pac-Man |
| **Inky** | 🔵 Cian | Usa la posición de Blinky para calcular una emboscada |
| **Clyde** | 🟠 Naranja | Persigue si está lejos, dispersa si está cerca |

En **modo asustado** (tras comer un power-up), todos los fantasmas se vuelven azules y huyen en direcciones aleatorias. Son vulnerables por unos segundos — parpadean en blanco cuando están a punto de recuperarse.

---

## 🕹️ Controles

| Acción | Teclado | Touch |
|---|---|---|
| Mover | `↑ ↓ ← →` o `WASD` | Deslizar en cualquier dirección |
| Pausar / Reanudar | `P` | — |
| Iniciar / Reiniciar | `Espacio` | Tocar pantalla |

---

## 🔢 Puntuación

| Objeto | Puntos |
|---|---|
| Punto (dot) | 10 pts |
| Power pellet | 50 pts |
| Fantasma asustado (1°) | 200 pts |
| Fantasma asustado (2°) | 400 pts |
| Fantasma asustado (3°) | 800 pts |
| Fantasma asustado (4°) | 1600 pts |

---

## 🖥️ Vista previa

```
┌─────────────────────────────────────────────────────┐
│  SCORE: 2340   NIVEL: 2   ●●●   HI: 2340            │
├─────────────────────────────────────────────────────┤
│  █████████████████████████████████████████████████  │
│  █ · · · · · · · █ · · · · · · · · · · · · · · █  │
│  █ ◉ █ █ · █ █ █ █ · █ █ · █ █ █ · █ █ ◉ █ █ █  │
│  █ · · · · · · · · · · · · · · · · · · · · · · █  │
│  █ · █ █ · █ · ██████ · █ · █ █ · █ █ · █ █ · █  │
│  █ · · · · █ · · · · · · · · · █ · · · · · · · █  │
│  ███████ · █ ██ ┌──────┐ ██ █ · █ ███████████ ███  │
│           · · · │ 👻👻 │ · · ·                     │
│  ███████ · █ ██ └──────┘ ██ █ · █ ███████████ ███  │
│  █ · · · · · · · · · · · · · · · · · · · · · · █  │
│  █ · █ ██████ █ ·  C  · · · · ·  · █ ██████ █ · █  │
│  █ · · · · · · · · · · ● · · · · · · · · · · · █  │
│  █████████████████████████████████████████████████  │
└─────────────────────────────────────────────────────┘
```

---

## 🚀 Uso

```bash
git clone https://github.com/Suarezsh/pacman-js.git
cd pacman-js

# Abrir en el navegador
start index.html        # Windows
open  index.html        # macOS / Linux
```

---

## 📁 Estructura

```
pacman-js/
└── index.html    ← Todo en un solo archivo (HTML + CSS + JS)
```

---

## 🛠️ Tecnologías

- **HTML5 Canvas 2D** — renderizado de laberinto, sprites y animaciones
- **JavaScript ES6+** — IA de fantasmas, física de movimiento, detección de colisiones
- **Web Audio API** — efectos de sonido procedurales
- **Google Fonts** — Press Start 2P (fuente retro pixelada)
- **Sin frameworks · Sin librerías · Sin npm**

---

## 📄 Licencia

MIT © [Suarezsh](https://github.com/Suarezsh)
