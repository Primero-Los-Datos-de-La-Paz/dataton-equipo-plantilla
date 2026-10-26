# Antes y después

La medición "antes" está en la carpeta `linea-base/` del paquete de tu desafío. Para el "después", usa **las mismas reglas**:

1. Copia el `reglas-calidad.yml` del paquete (si tiene uno) a `entrega/reglas-calidad.yml`.
2. Cambia en él los nombres de archivo del paquete (`data/interim/…`) por los de tu resultado (`salida/…`). No cambies las reglas.
3. Desde la raíz del repositorio:

```bash
python -m dataton scorecard entrega
python -m dataton nivel entrega
```

| Dimensión | Antes | Después | Qué cambió |
|---|---|---|---|
| Completitud | | | |
| Validez | | | |
| Unicidad | | | |
| Consistencia | | | |
| Territorialidad | | | |
| Documentación | | | |
| Nivel de la escala 0–7 | | | |

Exactitud y oportunidad no se miden de forma automática: si las mejoraste, explica cómo y con qué evidencia.
