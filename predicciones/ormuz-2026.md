# Predicción pre-registrada: cierre de Ormuz → IPC alimentario español

- **Pre-registrada:** 2026-07-04 (v1, en metodologia.html y el historial del
  repositorio privado).
- **Endurecida y congelada aquí:** 2026-07-10 (v2, este fichero), antes de
  conocer dato alguno de la ventana de resultado.
- **Adjudicación:** antes del 2027-07-31 se publicará ÉXITO o FALLO, en este
  repositorio y en <https://katastrofik.com/metodologia>, con la misma letra.

## Contexto

El estrecho de Ormuz está cerrado desde marzo de 2026. El índice Katastrofik
sostiene que ese shock de suministro se trasladará al precio de los alimentos
en España con el retraso propio de la cadena alimentaria (6-12+ meses,
medido en 2015-2026).

## Regla (v2, sin discreción)

**ÉXITO** si la variación anual del IPC español del grupo "Alimentos y
bebidas no alcohólicas" alcanza o supera el **4,7%** en **al menos un mes de
referencia de la ventana diciembre 2026 – junio 2027** (datos que el INE
publica entre enero y julio de 2027).

**FALLO** en cualquier otro caso.

Sin cláusula de atribución causal: la predicción es sobre el número, a secas.

## Detalle para que nadie tenga que fiarse

- **Serie:** INE, tabla 76125, serie "Nacional. Alimentos y bebidas no
  alcohólicas. Variación anual." — la misma que katastrofik.com publica como
  validación (`validation.ipc_food_es` en `data/latest.json`).
  Endpoint: <https://servicios.ine.es/wstempus/js/es/DATOS_TABLA/76125?tip=AM>
- **Umbral:** 4,7% = 2,7% (dato de marzo de 2026, mes del cierre de Ormuz)
  + 2,0 puntos porcentuales.
- **Vintage:** cuenta el dato definitivo que el INE publica para cada mes de
  referencia (a mediados del mes siguiente). Las revisiones posteriores no
  cambian el veredicto.
- **Agregación:** basta UN mes de la ventana en o por encima del umbral; no
  se promedia.
- **v1 → v2:** la v1 decía "una subida claramente atribuible, del orden de
  2 puntos o más". Era ambigua ("atribuible" no tiene árbitro; "del orden de"
  tampoco). Esta v2 la sustituye por un umbral numérico cerrado manteniendo
  la magnitud (+2,0 pp) y la ventana originales.
