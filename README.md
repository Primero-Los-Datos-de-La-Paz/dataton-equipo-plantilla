# Entrega de tu equipo

Este repositorio es **la entrega de tu equipo** en el datatón urbano de preparación de datos. No necesitas saber programar.

## Qué entregar, en 10 minutos

1. **Lee** las incidencias **Acuerdo de reglas de uso** y **Checklist de entrega** (pestaña *Issues*). Marca el acuerdo cuando todo el equipo esté de acuerdo.
2. **Completa [`autoria.yml`](autoria.yml)**: quiénes forman el equipo y si aceptan que su nombre aparezca en el reconocimiento público.
3. **Completa [`entrega/ficha-equipo.yml`](entrega/ficha-equipo.yml)**: desafío, ficha o indicadores y conjuntos trabajados.
4. **Pon tus datos de partida en [`entrega/datos/`](entrega/datos/)** (o un enlace con su suma SHA-256, si no se pueden copiar). **Nunca datos personales.**
5. **Deja tu procedimiento**, de una de estas formas:
   - scripts en [`entrega/scripts/`](entrega/scripts/) (Python, R…), un cuaderno, un historial de OpenRefine o un modelo de QGIS;
   - o los pasos que seguiste, uno por uno, en [`entrega/pasos-manuales.md`](entrega/pasos-manuales.md) (por ejemplo, en una hoja de cálculo).
6. **Pon tu resultado en [`entrega/salida/`](entrega/salida/)**, en formato abierto (CSV UTF-8, GeoJSON, GeoPackage…).
7. **Documenta:**
   - [`entrega/diccionario.csv`](entrega/diccionario.csv): una fila por columna;
   - [`entrega/procedencia.md`](entrega/procedencia.md): de dónde viene cada dato y qué cambiaste;
   - [`entrega/ficha-por-desafio.md`](entrega/ficha-por-desafio.md): lo que pide tu desafío;
   - [`entrega/antes-despues.md`](entrega/antes-despues.md): la medición antes y después.
8. **Guarda las sumas de tu resultado.** Desde la raíz del repositorio, con las herramientas instaladas:

   ```bash
   python -m dataton sumas entrega/salida
   python -m dataton validar .
   ```

   Si no puedes ejecutar comandos, pide a la organización que lo haga.

## Subir archivos sin usar Git

En GitHub, entra en la carpeta, pulsa **Add file → Upload files**, arrastra los archivos y pulsa **Commit changes**. Para editar un archivo de texto, ábrelo y pulsa el lápiz.

## Validación automática

Cada vez que subes cambios, la pestaña **Actions** comprueba la estructura de la entrega y busca posibles datos personales. Si aparece una cruz roja, abre el detalle para ver qué falta.

## Instalar las herramientas (opcional)

Se necesita Python 3.11 o más reciente. En Windows, cambia `source .venv/bin/activate` por `.venv\Scripts\Activate.ps1`.

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
pip install -e .
```

La carpeta `src/` contiene una copia de las herramientas del datatón: no necesitas modificarla.

## Reglas

- **Nunca subas datos personales** (nombres, cédulas, teléfonos, correos, fechas de nacimiento). Si subiste uno por error, **no basta con borrarlo**: avisa de inmediato al buzón institucional de la organización.
- **No republiques datos internos** fuera de este repositorio privado.
- **No edites el dato original:** los cambios van en el procedimiento y en la salida.
- **No inventes valores** ni rellenes brechas sin evidencia.
- **El repositorio es privado.** Al cierre, la organización lo congela con la etiqueta `entrega-final` y lo archiva (queda en solo lectura).
- **La licencia de los aportes de los equipos está pendiente** de la decisión institucional (ver [LICENSE](LICENSE)).
