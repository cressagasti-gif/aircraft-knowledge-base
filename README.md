<h1 align="center">Aircraft Knowledge Base</h1>
<p align="center">
  <b>Python · Jupyter Notebook</b><br>
  Interactive knowledge base of USAF fighter aircraft with fuzzy, case-insensitive search
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&labelColor=0D0D0D">
  <img src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&labelColor=0D0D0D">
</p>

---

## EN

An interactive knowledge base about United States Air Force fighter aircraft.

Aircraft are stored in a plain Python dictionary, and a lookup function answers
questions about a specific airframe. The search is **partial** and
**case-insensitive**, so `c-130`, `C-130` and `hercules` all resolve — and if a
query matches more than one entry the program asks you to narrow it down instead
of guessing.

### What it does

- Stores USAF fighter jets in a `fighter_jets` dictionary with structured fields:
  **role**, **key characteristic**, **generation**, **max speed** and
  **service ceiling**
- Provides `get_jet_info(query)` — partial, case-insensitive lookup
- Prompts for disambiguation when several aircraft match
- Ships with a short written introduction to the history of the USAF

### How to run

```bash
pip install jupyter
jupyter notebook USAF_proyecto.ipynb
```

Then edit the `query` cell at the bottom and run it. To add an aircraft, extend
the `fighter_jets` dictionary — the lookup picks it up with no other changes.

### Extending it

Everything lives in one dictionary, so extending the base is a matter of
appending a block in the same shape. Good next steps would be a
`pandas.DataFrame` instead of a dict, a CLI, or persistence to SQLite.

---

## ES

Base de conocimiento interactiva sobre aviones de combate de la Fuerza Aérea de
los Estados Unidos.

Los aviones se guardan en un diccionario de Python y una función de búsqueda
responde preguntas sobre un modelo concreto. La búsqueda es **parcial** e
**insensible a mayúsculas**, así que `c-130`, `C-130` y `hercules` dan el mismo
resultado — y si una consulta coincide con más de una entrada, el programa pide
que acotes en lugar de adivinar.

### Qué hace

- Guarda cazas de la USAF en un diccionario `fighter_jets` con campos
  estructurados: **rol**, **característica clave**, **generación**,
  **velocidad máxima** y **techo operativo**
- Ofrece `get_jet_info(query)` — búsqueda parcial e insensible a mayúsculas
- Pide precisión cuando varios aviones coinciden
- Incluye una breve introducción escrita a la historia de la USAF

### Cómo ejecutarlo

```bash
pip install jupyter
jupyter notebook USAF_proyecto.ipynb
```

Después editá la celda `query` del final y ejecutala. Para agregar un avión,
ampliá el diccionario `fighter_jets` — la búsqueda lo toma automáticamente sin
tocar nada más.

### Cómo extenderlo

Todo vive en un único diccionario, así que extender la base es agregar un bloque
con la misma forma. Buenos próximos pasos: usar `pandas.DataFrame` en vez de un
diccionario, una CLI, o persistencia en SQLite.

---

## Licencia

MIT — ver [LICENSE](LICENSE).
