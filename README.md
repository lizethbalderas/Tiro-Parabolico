## Descripción General 🎯

Apunta y **haz clic** para disparar un proyectil desde la esquina inferior izquierda.  
Balones azules aparecen desde la derecha y se desplazan hacia la izquierda.  
Tu objetivo es **impactarlos** con el proyectil en caída parabólica.

Esta versión agrega:
- **Movimiento más rápido** del **proyectil** y de los **balones**.  
- **Juego interminable**: cuando un balón sale de la ventana, **se re-posiciona** para continuar la partida.

---

## Contenido del Repositorio

- **cannon.py** → Script principal.  
  Maneja la creación y movimiento de balones, física del proyectil, detección de impactos, dibujo y ciclo de juego.

---

## Controles

| Acción | Cómo se hace |
|:------|:--------------|
| Disparar | **Clic** en cualquier punto de la ventana |
| Apuntar | Mueve el cursor y haz clic (la dirección/velocidad dependen del punto de clic) |

---

## Cambios Realizados🛠️

Se implementaron las siguientes mejoras sobre el juego base **Cannon (FreeGames)**:

1. **Más velocidad en proyectil y balones**  
   - Se incrementó la **velocidad inicial** del proyectil (componentes `speed.x` y `speed.y`).  
   - Se aumentó la **velocidad de desplazamiento** de los balones (decremento de `target.x` más grande por “tick”).  
   - Resultado: partidas **más dinámicas** y retadoras.

2. **Juego que nunca termina (reposición de balones)**  
   - Al detectar que un balón sale de la ventana, **se reubica** en la zona de entrada (derecha) con una **nueva altura aleatoria** para mantener la continuidad.  
   - Resultado: **modo infinito**, sin cortes de jugabilidad.

---
**Autores**

Lizeth Jaqueline Balderas Sánchez

Felipe Gutiérrez Herrera
