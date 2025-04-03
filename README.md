
# 📌 "Ahorca/World"

## 🎮 Introducción

Bienvenidos a la presentación del desarrollo de "Ahorca/World", un juego del ahorcado basada en mi propio diagrama entidad-relación. En esta presentación, se detalla cada uno de los componentes del sistema y su implementación en código Java con interfaz.

---


## 🚀 Implementación en Java con Interfaz

### 🔹 Tecnologías a Utilizar
- **Java** ☕
- **Swing** 🖥️ para la interfaz gráfica
- **AUN POR DECIDIR** 🗄️ para la conexión con base de datos
- **Visual Studio** 🏗️ para organizar el código

---

## 🗂️ 1.0 - Diagrama Entidad-Relación (E-R)

El diagrama E-R establece las relaciones entre los diferentes componentes del juego. A continuación, se explican las entidades principales:

![Tablero virtual con diagrama entidad-relación](https://github.com/user-attachments/assets/b86809e1-1c79-4da6-a3ba-6c0fe013cab6)

---

| Entidad       | Atributos                                      | Relación                                                                 |
|--------------|----------------------------------------------|------------------------------------------------------------------------|
| **Jugador (JUGADOR)** | Nombre 📝,  Contraseña 🔑,  IDJugador 🆔,  IDAdmin 🛡️ (opcional) | Puede jugar varias partidas 🎲, obtener logros 🏆, aparecer en el ranking 📊 |
| **Administrador (ADMIN)** | IDAdmin 🆔, Rango ⭐, IDJugador 🆔 | Solo los jugadores con la contraseña de admin pueden acceder al rango |
| **Partida (PARTIDA)** | IDPartida 🆔, Resultado ✅❌, Puntuación 🎯, IDJugador 🆔, IDPalabra 🔤, IDJuego 🕹️ | Cada jugador puede participar en múltiples partidas; cada partida tiene una palabra asociada |
| **Logros (LOGROS)** | IDLogro 🆔, IDJugador 🆔 | Cada jugador puede desbloquear varios logros |
| **Ranking (RANKING)** | IDRanking 🆔, Rango 🏅, IDPartida 🆔 | Cada partida tiene una puntuación que influye en el ranking |
| **Palabra (PALABRA)** | IDPalabra 🆔, Sinónimo 1 📝, Sinónimo 2 📝, IDDificultad 🔥 | Cada palabra tiene una dificultad asignada |
| **Dificultad (DIFICULTAD)** | IDDificultad 🆔, Nivel 📶, Recompensa 🎁 | A mayor dificultad, mayor puntuación obtenida |
| **Modo de Juego (MODOJUEGO)** | IDJuego 🆔, Dificultad 🔥 | Cada partida pertenece a un modo de juego determinado |

---

🎯 ** 2.0 - Próximo paso:** Desarrollar la base de datos y conectar con el código Java. 

¡Os mantendre informados! 💻🔥

