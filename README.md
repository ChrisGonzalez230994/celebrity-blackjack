<div align="center">

# 🎰 Celebrity Age Blackjack

<img src="https://img.shields.io/badge/Estado-En%20Producción-brightgreen?style=for-the-badge&logo=netlify" />
<img src="https://img.shields.io/badge/Versión-2.0-gold?style=for-the-badge" />
<img src="https://img.shields.io/badge/Licencia-MIT-blue?style=for-the-badge" />
<img src="https://img.shields.io/badge/Jugadores-1--5-purple?style=for-the-badge&logo=game-controller" />

<br/>

> ### *¿Cuántos años tiene tu famoso favorito?*
> **El juego de Blackjack donde tu límite no es 21... sino lo que vos mismo estimás.**

<br/>

[![Jugar Ahora](https://img.shields.io/badge/🎮%20JUGAR%20AHORA-FF6B6B?style=for-the-badge&logoColor=white)](https://celebrityblackjack.netlify.app)

---

</div>

## 📖 ¿De qué se trata?

**Celebrity Age Blackjack** es un juego multijugador de estimación de edades inspirado en el Blackjack clásico. En lugar de intentar llegar a 21, cada jugador construye su propio límite personal —el **"Pozo"**— estimando las edades de 4 celebridades famosas, y luego intenta acercarse a ese límite sin pasarlo.

¿Sos bueno adivinando edades? ¡Demostralo! 🏆

---

## 🎮 Modos de Juego

<div align="center">

| Modo | Descripción | Jugadores |
|------|------------|-----------|
| 👥 **Multijugador** | Hasta 5 personas, cada una con su propio Pozo y cartas únicas | 2 – 5 |
| 🤖 **Vs IA** | Enfrentate a Claude, que estima y decide en tiempo real | 1 vs IA |
| 🎯 **Solo** | Practicá tu intuición contra tu propio Pozo | 1 |

</div>

---

## 🃏 ¿Cómo se juega?

```
FASE 1 — EL POZO                    FASE 2 — LA PARTIDA
━━━━━━━━━━━━━━━━━━━                 ━━━━━━━━━━━━━━━━━━━━━
  📸 Se muestran 4 celebridades       🃏 Te salen celebridades únicas
  ✏️  Estimás la edad de cada una      🔢 Estimás la edad en tiempo real
  ➕  La suma = tu POZO personal       ⚖️  Decidís: ¿tomo otra carta?
  🔒  Ese es tu límite secreto         🛑  Plantate antes de pasarte
                                       🏆  El más cercano a su Pozo gana
```

### 🏁 Al final de cada ronda
- Se revelan las **edades reales** de las 4 celebridades del Pozo
- Se compara tu **Pozo estimado** vs el **Pozo real**
- Se muestra carta por carta: tu estimación, la edad real y la diferencia
- Se hace el **ranking** de quién se acercó más sin pasarse

---

## ✨ Características

- 🌟 **+300 celebridades** de todas las categorías
- 📸 **Fotos reales** cargadas automáticamente desde Wikipedia
- 🤖 **IA conectada a Claude** que razona y comenta cada jugada
- 📊 **Pantalla de resultados** con comparativa detallada de estimaciones
- 📱 **100% responsive** — funciona en celular, tablet y computadora
- ⚡ **Sin instalación** — corre directo en el navegador
- 🆓 **Completamente gratuito**

---

## 🌟 Celebridades incluidas

<div align="center">

| Categoría | Ejemplos |
|-----------|---------|
| 🎤 Música Pop / Urbano | Taylor Swift, Bad Bunny, Karol G, Bizarrap, Peso Pluma |
| 🎬 Actores / Actrices | Zendaya, Timothée Chalamet, Pedro Pascal, Margot Robbie |
| ⚽ Deportes | Messi, Mbappé, LeBron James, Alcaraz, Haaland |
| 🧽 Personajes Animados | Homer Simpson, Goku, Mickey Mouse, SpongeBob, Pikachu |
| 👴 Edad Avanzada | Clint Eastwood (94), Warren Buffett (94), Paul McCartney (83) |
| 🇦🇷 Latinoamérica | María Becerra, Wos, Nicki Nicole, Paulo Londra, Tini |
| 🎮 Streamers / Influencers | MrBeast, Ibai Llanos, Khaby Lame, Pokimane |
| 👑 Realeza / Política | Rey Carlos III, Príncipe William, Meghan Markle |

</div>

---

## 🛠️ Tecnologías

<div align="center">

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Claude AI](https://img.shields.io/badge/Claude%20AI-CC785C?style=for-the-badge&logo=anthropic&logoColor=white)
![Wikipedia API](https://img.shields.io/badge/Wikipedia%20API-000000?style=for-the-badge&logo=wikipedia&logoColor=white)
![Netlify](https://img.shields.io/badge/Netlify-00C7B7?style=for-the-badge&logo=netlify&logoColor=white)

</div>

---

## 🚀 Instalación y uso local

### Opción A — Sin instalación (recomendado)
Simplemente abrí el archivo `index.html` en cualquier navegador moderno. ¡No necesitás servidor ni dependencias!

### Opción B — Clonar el repositorio
```bash
# 1. Cloná el repo
git clone https://github.com/TU-USUARIO/celebrity-blackjack.git

# 2. Entrá a la carpeta
cd celebrity-blackjack

# 3. Abrí el archivo en tu navegador
open index.html        # macOS
start index.html       # Windows
xdg-open index.html    # Linux
```

---

## 🔑 Configuración de la API Key

El modo **Vs IA** requiere una API Key de Anthropic (Claude). Para obtenerla:

1. Registrate gratis en [console.anthropic.com](https://console.anthropic.com)
2. Andá a **API Keys** → **Create Key**
3. En el archivo `index.html`, buscá las líneas con `fetch("https://api.anthropic.com/v1/messages"` y agregá tu key en los headers:

```javascript
headers: {
  "Content-Type": "application/json",
  "x-api-key": "TU-API-KEY-AQUÍ",              // ← agregá esta línea
  "anthropic-version": "2023-06-01"             // ← y esta
}
```

> ⚠️ **Nota de seguridad:** La API Key solo es visible para quien acceda al código fuente. Para uso entre amigos o familiar está perfecto. Para un sitio público masivo, se recomienda un backend intermediario.

---

## 📁 Estructura del proyecto

```
celebrity-blackjack/
│
├── 📄 index.html          # El juego completo (HTML + CSS + JS en un solo archivo)
└── 📄 README.md           # Este archivo
```

> Todo el juego está contenido en un **único archivo HTML** de ~1.400 líneas, sin dependencias externas ni librerías que instalar.

---

## 🎯 Roadmap — Próximas mejoras

- [ ] 🔊 Efectos de sonido y música de fondo
- [ ] 🏆 Tabla de puntuaciones histórica
- [ ] 🌍 Más celebridades de cada región
- [ ] 📱 App móvil nativa
- [ ] 🎨 Temas visuales alternativos (día / noche)
- [ ] 🔗 Modo online multijugador en tiempo real

---

## 🤝 Contribuciones

¿Querés agregar celebridades, reportar un bug o sugerir mejoras?

1. Hacé un **Fork** del repositorio
2. Creá una nueva rama: `git checkout -b feature/nueva-celebridad`
3. Hacé tus cambios y commiteá: `git commit -m "Agrego nuevas celebridades 2025"`
4. Pusheá: `git push origin feature/nueva-celebridad`
5. Abrí un **Pull Request**

---

## 📜 Licencia

```
MIT License — Libre para usar, modificar y distribuir.
```

---

<div align="center">

### Hecho con ❤️ y mucho ☕ en Argentina 🇦🇷

**¿Te gustó el proyecto? ¡Dejá una ⭐ en el repo!**

<br/>

![Visitors](https://img.shields.io/badge/Jugadores%20Totales-Infinitos-gold?style=for-the-badge&logo=game-controller)

<br/>

`#javascript` `#html` `#css` `#game` `#blackjack` `#celebrities` `#claudeai` `#anthropic` `#argentina` `#proyecto` `#juego` `#trivia` `#famosos`

</div>
