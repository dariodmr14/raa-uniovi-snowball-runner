# ❄️ Snowball Runner

> 🎓 **Realidad y Accesibilidad Aumentadas (RAA)** · Universidad de Oviedo · Curso 2026/2027
> Práctica **Ball Runner** (Unity 2020.3.49f1)

Eres una bola de nieve que baja por una montaña helada: rueda por la nieve para crecer, esquiva la lava que te derrite y usa tu tamaño para superar los obstáculos.

## 🎬 Vídeo

▶️ **[Ver el vídeo en YouTube](https://youtu.be/3oPaEL-benI)** · #RAAUniovi2026

## 🎮 Cómo jugar

Ejecuta `Build/Snowball Runner.exe` (Windows).

| Tecla | Acción |
|---|---|
| WASD / Flechas | Moverse |
| Espacio | Saltar |
| Enter | Saltar la cinemática inicial |

**Objetivo:** recoger los 5 copos de nieve antes de que se acabe el tiempo.
**Pierdes si:** se acaba el tiempo o te derrites del todo. Si caes al lago helado, el nivel se reinicia.

## ⚙️ Mecánicas

- **Tamaño variable:** la bola crece al rodar por las zonas de nieve (solo si se mueve) y se derrite en la lava. El tamaño cambia su escala y su masa: grande es más pesada y salta menos.
- **Obstáculos según el tamaño**, hechos solo con geometría y física (sin código):
  - Copo en lo alto → hay que ser **grande** para alcanzarlo.
  - Túnel y techo bajo → hay que ser **pequeño** para pasar.
  - Rejilla de barras → la bola pequeña cae por los huecos, la **grande** pasa por encima.
- **HUD** con tamaño (%), copos recogidos y tiempo, con avisos en rojo.
- **Escenas:** menú → instrucciones → nivel con cinemática → victoria / derrota.

## 🧩 Programación (scripts C#)

| Script | Función |
|---|---|
| `MoveSnowball` | Movimiento con fuerzas, velocidad máxima y salto |
| `SnowballSize` | Crecer / derretirse con las zonas, escala, masa y sonidos |
| `SnowballGame` | Copos, temporizador, HUD, victoria y derrota |
| `CameraFollow` | Cámara que sigue a la bola y se aleja al crecer |
| `LakeRestart` | Reinicio del nivel al caer al lago |
| `CinematicIntro` | Cinemática inicial (se salta al reiniciar por caída) |
| `MenuScript` | Navegación entre escenas y salir del juego |
| `Rotate` | Rotación de los copos |

## 🎨 Recursos

- Texturas: [ambientCG](https://ambientcg.com) (CC0)
- Sonidos y música: [Pixabay](https://pixabay.com)
- Fuente: [Fredoka](https://fonts.google.com/specimen/Fredoka) (OFL)

## 📁 Contenido del repositorio

```
BolaDeNieve/  → proyecto de Unity 2020.3.49f1
Build/        → ejecutable para Windows
```

## 👤 Autor

**Darío Morales Riega** · Grado en Ingeniería Informática del Software, Universidad de Oviedo

---

*Este README ha sido generado con ayuda de IA.*
