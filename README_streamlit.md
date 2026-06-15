# Diseño de muro estructural - Streamlit

## Ejecución

```bash
pip install -r requirements.txt
streamlit run streamlit_app.py
```

## Cambios incorporados

Esta versión agrega:

1. **Validación de espesor mínimo**
   - mínimo general: 20 cm,
   - mínimo con elementos especiales de borde: 25 cm,
   - mínimo con vigas de acople: 35 cm,
   - validación por altura no apoyada: `hw/N/16`.

2. **Tipo de análisis para cortante**
   - fuerza lateral equivalente: `ω = 1.3 + N/30`,
   - análisis modal espectral: `ω = 1.2 + N/50`.

3. **Tres modos de falla por cortante en memoria**
   - tensión diagonal,
   - compresión diagonal,
   - deslizamiento.

4. **Memoria Word dinámica**
   - redacta paso a paso el cálculo,
   - incluye validación de espesor,
   - incluye imágenes del muro,
   - se actualiza según los datos ingresados.
