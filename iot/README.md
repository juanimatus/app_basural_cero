# 🔌 Módulo IoT – Sensado Ambiental para Basural Cero

Este módulo contiene el firmware y la lógica de conexión de sensores al microcontrolador **ESP32**, utilizado para detectar condiciones críticas en zonas con basurales informales.

---

## 🧪 Sensores utilizados

| Sensor        | Propósito                            |
|---------------|---------------------------------------|
| **DHT11/DHT22** | Temperatura y humedad relativa       |
| **MQ-135**     | Gases tóxicos / calidad del aire     |
| **LDR / IR**   | Detección de humo o cambios de luz   |

---

## 🔧 Componentes mínimos

- ESP32 DevKit v1
- Sensor DHT11 o DHT22
- Sensor MQ-135
- Jumpers, protoboard
- Conexión Wi-Fi activa (o alternativa: ESP-NOW)

---

## 🧠 Lógica del sistema

- Lectura cada 5 minutos
- Si supera umbral crítico de gases → genera **alerta**
- Los datos se envían a un servidor vía **HTTP POST** o MQTT
- Opcional: encendido de LED local o mensaje en pantalla OLED

---

## 📤 Ejemplo de payload

```json
{
  "ubicacion": "Palmira_Mendoza",
  "temperatura": 28.4,
  "humedad": 63.2,
  "gas_ppm": 435,
  "alerta": true,
  "timestamp": "2025-06-21T14:50:00"
}
