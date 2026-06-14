# Diseño de muro estructural - Streamlit

## Ejecución

```bash
pip install -r requirements.txt
streamlit run streamlit_app_hx_auto_manual.py
```

## Cambio incorporado

Ahora la app permite escoger cómo usar `hx`:

1. **Calcular hx automáticamente**
   - Usa `lbe`, `bw`, recubrimiento/posición de barras, barras intermedias en X y barras intermedias en Y.

2. **Ingresar hx manualmente**
   - Útil cuando el detalle real tiene más vinchas, ganchos o ramales que reducen la separación entre barras longitudinales soportadas lateralmente.
   - En este modo ingresas directamente el `hx` real medido del detalle.

En la memoria se reportan:

- modo de hx,
- hx automático estimado,
- hx usado para el cálculo,
- separación en X,
- separación en Y,
- espaciamiento de estribos,
- Ash requerido.
