# PMD2 AG News - CRISP-DM NLP

Notebook principal:

```text
PMD2_AG_News/pmd2_ag_news_crispdm_nlp.ipynb
```

Para la entrega en Colab, abrir el notebook y ejecutar todas las celdas con
`FAST_MODE=False` (valor por defecto cuando no existe la variable de entorno
`PMD2_FAST_VALIDATE`). La validacion local se hizo con `PMD2_FAST_VALIDATE=1`
para usar un subconjunto estratificado y comprobar que toda la ruta ejecuta.

Entorno local recomendado:

```powershell
C:\Users\ASUS\.venvs\pmd2-ag-news-py312\Scripts\activate
python -m nbconvert --to notebook --execute --inplace PMD2_AG_News\pmd2_ag_news_crispdm_nlp.ipynb
```

Se instalo Python 3.12 en el usuario y se creo el venv:

```text
C:\Users\ASUS\.venvs\pmd2-ag-news-py312
```

Dependencias verificadas en ese entorno:

- `tensorflow 2.21.0`
- `xgboost 3.3.0`
- `datasets 5.0.0`
- `scikit-learn 1.9.0`

Motivo: el Python global del equipo es 3.14 y TensorFlow no publica wheel
compatible para esa version. Por eso se usa Python 3.12 en un entorno virtual.

El notebook cubre las semanas 9 a 15 del PMD2: XGBoost/boosting, MLP,
Keras/TensorFlow, clustering, Naive Bayes, optimizacion, ensamblajes y NLP. No
incluye Computer Vision porque el dataset AG News es exclusivamente textual.
