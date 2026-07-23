# Katastrofik

# 80.51  ·  CRISIS
### 23 de julio de 2026

Índice de tensión de la cesta de la compra española. De 0 a 100.
Cada mañana se publica aquí la lectura del día.

Hoy pesa sobre todo el gas: las reservas de Europa están muy bajas para la época.

**calma** 0-25 · **atención** 25-50 · **alerta** 50-75 · **crisis** más de 75

---

### Los datos

- **[`data/today.json`](data/today.json)** — la lectura de hoy. Empieza por aquí.
- **[`data/history.json`](data/history.json)** — todas las lecturas.
- `data/latest.json` — la de hoy con todo el detalle.
- `data/ranges.json` y `data/buffer_seasonal.json` — la calibración del motor.
- `predicciones/` — predicciones escritas antes de saber el resultado.

Desde el **2 de julio de 2026** el índice funciona con un motor nuevo, con más
sensores y mejor calibrado. Lo anterior se calculó con el motor viejo y no es
directamente comparable; cada lectura lleva su `engine_version`.

El índice busca detectar la presión antes de que llegue del todo al precio
final. Cuánto se adelanta todavía lo estamos midiendo.

[katastrofik.com](https://katastrofik.com)
