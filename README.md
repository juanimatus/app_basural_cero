# 🌍 AIconcagua: Mendoza sin Basura – Plataforma de Intervención Ambiental Inteligente

AIconcagua: Mendoza sin Basura, es una iniciativa tecnológica-social pensada para combatir los basurales informales en zonas urbanas y rurales. Integra sensores IoT, mapas interactivos y participación vecinal para detectar, mapear y erradicar focos contaminantes con una mirada comunitaria y sostenible.

---

## 🚀 Funcionalidades principales

- 🗺️ **Mapa interactivo** de basurales y su evolución
- 🧑‍🤝‍🧑 **Reportes vecinales** con validación por comunidad o municipio
- 🔔 **Alertas automáticas** mediante sensores ambientales (gas, temperatura, humedad)
- 📊 **Panel de estadísticas** por zona, evolución histórica y estado
- 📱 Interfaz amigable, pensada para que cualquier vecino pueda participar

---

## 🧠 Motivación

En muchas zonas vulnerables, los basurales informales generan contaminación, enfermedades y pérdida de espacios públicos. Este proyecto busca integrar tecnología con acción comunitaria, empezando por casos reales de Mendoza (Argentina), donde hay barrios enteros afectados.

---

## 🧰 Stack Tecnológico

| Componente      | Tecnología                      |
|-----------------|----------------------------------|
| Frontend        | React + Leaflet.js               |
| Backend         | Node.js + Express                |
| Base de datos   | MongoDB                          |
| IoT             | ESP32 + sensores DHT11 / MQ-135 |
| Hosting         | Firebase / GitHub Pages (prototipo) |

---

## 🏗️ Estructura del proyecto

```bash
app_basural_cero/
├── frontend/         # React + Leaflet
├── backend/          # Node.js API + MongoDB
├── iot/              # Scripts para sensores ESP32
├── comunidad/        # Manuales, afiches y estrategia de difusión
└── docs/             # Wireframes, base de datos y propuestas institucionales
