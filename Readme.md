# Price Metals

## Objetivo
Calcular el precio tentativo de una joya basado en los metales que contiene, considerando cantidad y precio actual de cada metal, además de un margen de trabajo de joyería.

---

## Metodología

1. **Identificar los metales preciosos** de la joya:
   - Oro (XAU)
   - Plata (XAG)
   - Platino (XPT)
   - Otros metales si aplica

2. **Registrar la cantidad de cada metal** (en gramos o onzas).

3. **Obtener el precio actual** de cada metal:
   - Se puede usar una API de metales preciosos (por ejemplo, [Metals-API](https://metals-api.com)).

4. **Calcular el precio base de cada metal**:

   PrecioMetal = Cantidad × PrecioUnitario

5. **Sumar los precios de todos los metales** para obtener el precio total base:

   PrecioBase = PrecioMetal1 + PrecioMetal2 + ...

6. **Aplicar un margen de joyería** (por diseño, trabajo y ganancia):

   PrecioFinal = PrecioBase × (1 + Margen)

---

## Ejemplo

### Datos de la joya

| Metal | Cantidad (g) | Precio por g (USD) |
|-------|--------------|------------------|
| Oro   | 5            | 60               |
| Plata | 10           | 0.75             |

### Cálculo

- Oro: 5 × 60 = 300 USD  
- Plata: 10 × 0.75 = 7.5 USD  
- Precio base total = 307.5 USD  
- Margen 20% → Precio final = 307.5 × 1.2 = 369 USD

---

## Consideraciones

- Los precios de los metales pueden variar diariamente, por lo que se recomienda **usar datos actualizados**.  
- El margen puede ajustarse según el diseño, trabajo artesanal o comercialización de la joya.  
- Para proyectos reales, se puede automatizar la obtención de precios mediante **API** y generar reportes dinámicos.

---

## Referencias

- [Metals-API](https://metals-api.com) – API para precios de metales precioso
