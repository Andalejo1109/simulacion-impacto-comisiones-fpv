# Simulación: Impacto de Comisiones en FPV vs ETFs de Bajo Costo

Ejemplo práctico del efecto de las comisiones de administración y el impuesto a la ganancia ocasional en una inversión a largo plazo.

## Escenario

| Parámetro | Valor |
|-----------|-------|
| Aporte mensual | $1.000.000 COP |
| Horizonte | 15 años |
| Rentabilidad bruta | 15% anual |
| Comisión FPV | 3.5% anual |
| Comisión ETFs | 0.05% anual |

## Tratamiento tributario de las ganancias al retirar

| Vehículo | Tratamiento de las ganancias al retirar / vender | Condición |
|----------|--------------------------------------------------|
| **FPV** | Exento (ni capital ni rendimientos) | Si cumples 10 años, pensión, vivienda, etc. |
| **BVC** (acciones listadas) | Exento (no es renta ni ganancia ocasional) | Si no vendes más del 3% de las acciones en circulación de esa sociedad en el año (Art. 36-1 ET). Para un inversionista normal, casi siempre se cumple. |
| **eToro / extranjero** | Ganancia ocasional al 15% | Si se mantiene ≥ 2 años y se considera activo fijo. Si se vende antes de 2 años, puede ser renta ordinaria (hasta 39%). |

## Impacto en el escenario de 15 años

| Escenario | Valor final | Impuesto sobre ganancias | Valor neto final |
|-----------|-------------|---------------------------|------------------|
| FPV (3.5% comisión) | ~$476 millones | $0 (si cumple condiciones) | **~$476 millones** |
| eToro (0.05% comisión) | ~$665 millones | ~$73 millones (15%) | **~$592 millones** |
| BVC (si aplica Art. 36-1) | ~$665 millones | $0 | **~$665 millones** |

Incluso pagando el 15% de ganancia ocasional en eToro, el resultado neto (~$592 millones) sigue siendo ~24% superior al FPV (~$476 millones). La diferencia es de unos **$116 millones** a favor de la autoinversión de bajo costo.

## Resumen práctico

- La comisión del **3.5%** del FPV sigue siendo el factor que más destruye el resultado a largo plazo.
- El beneficio de no pagar ganancia ocasional en el FPV (o en la BVC) no alcanza a compensar ese costo de comisión tan alto.
- Entre eToro (con 15%) y BVC (potencialmente exento), la BVC es más eficiente tributariamente para acciones colombianas, siempre que no superes el límite del 3%.
- Cuando el cupo de renta exenta ya está lleno, el beneficio adicional de meter más dinero al FPV es limitado, mientras que el costo de la comisión es permanente.

**Conclusión**: incluso considerando el 15% de ganancia ocasional en eToro, sigue siendo más conveniente invertir por tu cuenta en ETFs de bajo costo que pagar 3.5% de comisión en un FPV, a menos que la comisión real de tu fondo sea significativamente más baja (idealmente ≤ 1.5–2%).

## Cómo usar

1. Clona el repositorio.
2. Abre `simulacion_comisiones.ipynb` en Jupyter o Google Colab.
3. Ejecuta las celdas para ver los gráficos y tablas (incluye gráfico de barras del valor neto final).

---

*Este es un ejemplo ilustrativo. Los resultados dependen de la rentabilidad real, las comisiones exactas de cada fondo y la situación tributaria particular de cada persona.*
