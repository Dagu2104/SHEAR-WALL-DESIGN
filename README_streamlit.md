# Diseño de muro estructural - Streamlit

## Ejecución

```bash
pip install -r requirements.txt
streamlit run streamlit_app.py
```

## Cambio incorporado

Se agregó la revisión de **deslizamiento en juntas horizontales de construcción** para muros fundidos por etapas verticales.

La app permite ingresar:

- altura máxima de vaciado vertical,
- tipo de superficie de junta,
- coeficiente de fricción μ,
- factor φ para deslizamiento,
- si se usa Vu amplificado o Vu_junta manual,
- si se usa Pu o Nu_junta manual.

El campo `Coeficiente de fricción μ` incluye ayuda con signo de interrogación en Streamlit; al pasar el mouse se muestran los valores orientativos de rugosidad usados por la app.
