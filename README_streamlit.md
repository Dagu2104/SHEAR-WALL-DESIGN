# Diseño de muro estructural - Streamlit

## Ejecución

```bash
pip install -r requirements.txt
streamlit run streamlit_app_hx_s_corregido.py
```

## Corrección incorporada

Se corrigió el cálculo de la separación de estribos cuando `hx` resulta grande.

Antes, la expresión:

```text
s0 = 100 + (350 - hx) / 3
```

podía dar negativa si `hx > 650 mm`.

Ahora se limita `s0` entre 100 mm y 150 mm:

```text
s0_bruto = 100 + (350 - hx) / 3
s0_usado = min(150, max(100, s0_bruto))
```

Luego:

```text
s = min(bw/4, 6db longitudinal, s0_usado)
```

La memoria reporta qué límite controla la separación.
