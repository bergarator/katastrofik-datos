# Katastrofik

# 83.16  ·  CRISIS
### 29 de octubre de 2026

Katastrofik es un índice diario, de 0 a 100, de la tensión mundial (energía,
alimentos, transporte, geopolítica) que acaba llegando a los precios en España.
Cada mañana se publica aquí la lectura del día.

**calma** 0-25 · **atención** 25-50 · **alerta** 50-75 · **crisis** más de 75

---

### Los datos

- **[`data/today.json`](data/today.json)** — la lectura de hoy. Empieza por aquí.
- **[`data/history.json`](data/history.json)** — todas las lecturas.
- **[`data/history_provenance.jsonl`](data/history_provenance.jsonl)** — qué es cada lectura: sellada aquí
  en vivo (con su commit), solo en el repo privado, del motor viejo o cálculo hacia atrás.
- `data/latest.json` — la de hoy con todo el detalle.
- `data/ranges.json` y `data/buffer_seasonal.json` — la calibración del motor.
- `predicciones/` — predicciones escritas antes de saber el resultado.
- `sellos/` — huellas, con fecha, de las previsiones aún no publicadas.

Desde el **2 de julio de 2026** el índice funciona con un motor nuevo, con más
sensores y mejor calibrado, y desde el **23 de julio** cada lectura queda sellada
aquí con su fecha: ese es el historial en vivo (`clase: v3_publica` en el fichero de
procedencia). Lo anterior se calculó con el motor viejo o hacia atrás: no es historial
en vivo ni es directamente comparable, y el campo `version` (`v2` en todas las filas)
no lo distingue; el fichero de procedencia, sí.

El índice busca detectar la presión antes de que llegue del todo al precio
final. Cuánto se adelanta todavía lo estamos midiendo.

[katastrofik.com](https://katastrofik.com)
