# Diseño de muro estructural - Streamlit

## Ejecución

```bash
pip install -r requirements.txt
streamlit run streamlit_app.py
```

## Cambio incorporado

La app ahora genera una **memoria de cálculo en Word (.docx)** con redacción paso a paso.

La memoria incluye texto dinámico según los datos ingresados:

- nombre del proyecto,
- identificación del muro,
- ejes,
- niveles,
- geometría,
- materiales,
- solicitaciones,
- revisión por cortante,
- flexo-compresión,
- elementos de borde,
- acero distribuido del alma,
- conclusiones,
- e imágenes del corte longitudinal y corte transversal.

En el ZIP, el archivo principal se llama `streamlit_app.py` para usarlo directamente en Streamlit Cloud.
