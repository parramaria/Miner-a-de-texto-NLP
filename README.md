# Minería de Texto y Procesamiento de Lenguaje Natural (NLP) con Stanza

Este proyecto fue desarrollado como parte del curso **EC0323-DS1-202501**, y tiene como objetivo aplicar técnicas de minería de texto y procesamiento de lenguaje natural utilizando la biblioteca `stanza` de Stanford NLP.

## Archivos del proyecto

- `Trabajo_NLP.ipynb`: Notebook con todo el análisis paso a paso.
- `texto1.txt`: Primer texto analizado (mínimo 1000 palabras).
- `texto2.txt`: Segundo texto analizado.
- `README.md`: Este archivo con explicación del trabajo y resultados.

## Herramientas utilizadas

- Python 3.10+
- [Stanza (Stanford NLP)](https://stanfordnlp.github.io/stanza/)
- NLTK (para stopwords)
- WordCloud y Matplotlib (para visualización)
- Jupyter Notebook

## Pasos realizados

1. **Carga de datos**  
   Se cargaron dos textos desde archivos `.txt`, cada uno con al menos 1000 palabras.

2. **Limpieza y normalización**  
   - Eliminación de HTML, URLs, puntuación, emojis y espacios extra.
   - Conversión a minúsculas.

3. **Análisis básico (sin NLP)**  
   - Conteo de párrafos, oraciones y palabras por texto.
   - Comparación de longitud y complejidad general.

4. **Procesamiento con Stanza**  
   - Tokenización, eliminación de *stopwords* y lematización.
   - Extracción de las palabras más frecuentes.
   - Generación de nubes de palabras para comparación temática.

5. **Etiquetado gramatical (POS tagging)**  
   - Identificación de sustantivos, verbos y adjetivos más frecuentes.
   - Análisis de categorías dominantes en cada texto.

6. **Extracción de tripletas SVO (Sujeto-Verbo-Objeto)**  
   - Se identificaron relaciones básicas entre sujetos, acciones y objetos.
   - Se analizaron patrones que sugieren afirmaciones comunes u opiniones.

## Hallazgos principales

- **Texto 1:**  
  Predominan los **sustantivos abstractos** y **verbos en pasado**, lo que sugiere una narrativa enfocada en hechos o eventos pasados. Las palabras frecuentes como “gobierno”, “sociedad” y “cambio” indican un enfoque sociopolítico.

- **Texto 2:**  
  Contiene más **adjetivos calificativos** y **verbos en presente**, lo que sugiere una estructura más descriptiva. Los términos como “vida”, “emociones” y “personas” sugieren un enfoque más personal o literario.

- **Tripletas SVO comunes:**  
  - “El autor explica el fenómeno”
  - “La sociedad enfrenta problemas”
  - “El texto transmite emociones”

