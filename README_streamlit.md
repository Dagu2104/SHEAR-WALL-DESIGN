# Diseño de muro estructural - Streamlit

## Ejecución

```bash
pip install -r requirements.txt
streamlit run streamlit_app_hx_recubrimiento_puro.py
```

## Cambio incorporado

La app ahora pide el **recubrimiento libre/puro** del cabezal o muro, por ejemplo 4 cm.

Para calcular hx automático, el programa calcula internamente:

```text
distancia al centro de barra extrema =
recubrimiento libre + Ø estribo + Ø barra longitudinal / 2
```

Luego calcula:

```text
separación en X = (lbe - 2·distancia_centro_barra) / (n_intermedias_x + 1)
separación en Y = (bw - 2·distancia_centro_barra) / (n_intermedias_y + 1)
hx = mayor separación entre X e Y
```

También se mantiene la opción de ingresar `hx` manualmente cuando el detalle real tenga vinchas, ganchos o ramales adicionales.
