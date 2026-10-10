# Simulación: Impacto de Comisiones en FPV vs ETFs de Bajo Costo

Ejemplo práctico del efecto de las comisiones de administración y el impuesto a la ganancia ocasional en una inversión a largo plazo.

> **Disclaimer**: Esta simulación asume que los tres vehículos (FPV, eToro y BVC) invierten en el **mismo tipo de activo subyacente**: ETFs globales de bajo costo. La diferencia principal analizada es el costo de comisión y el tratamiento tributario al retirar, no la rentabilidad bruta del portafolio.

## Escenario

| Parámetro | Valor |
|-----------|-------|
| Aporte mensual | $1.000.000 COP |
| Horizonte | 15 años |
| Rentabilidad bruta | 15% anual |
| Comisión FPV | 3.5% anual |
| Comisión ETFs | 0.05% anual |

> **Nota sobre la rentabilidad**: El 15% bruto anual usado en esta simulación es conservador. El portafolio real en eToro ha obtenido una rentabilidad promedio de **23.5% anual** en los últimos 4 años.  
> Perfil: https://www.etoro.com/people/andalejo1109

## Cómo se cobra la comisión del FPV

La comisión del 3.5% se cobra sobre el **saldo** (activos bajo administración), no sobre el aporte ni sobre la rentabilidad.

- Se liquida diariamente sobre el saldo del día anterior.
- Ejemplo: con un saldo de $100 millones y comisión del 3.5% EA, el costo anual aproximado es de $3.5 millones (antes del crecimiento del saldo).
- No es un cargo único al aportar ni un porcentaje de la ganancia.

Esto hace que el impacto sea fuerte a largo plazo: el porcentaje se resta del saldo todos los años, gane o pierda el fondo.

## Resultados brutos (impacto de las comisiones)

| Concepto | FPV (3.5%) | ETFs (0.05%) |
|----------|------------|--------------|
| Total aportado | $180.000.000 | $180.000.000 |
| Valor final | aprox. $476 millones | aprox. $665 millones |
| Ganancias | aprox. $297 millones | aprox. $485 millones |
| Diferencia | — | **+$189 millones** |

La comisión del 3.5% se come aproximadamente el **39% de las ganancias potenciales**.

## Tratamiento tributario de las ganancias al retirar

| Vehículo | Tratamiento de las ganancias al retirar / vender | Condición |
|----------|--------------------------------------------------|-----------|
| **FPV** | Exento (ni capital ni rendimientos) | Si cumples 10 años, pensión, vivienda, etc. |
| **BVC** (acciones listadas) | Exento (no es renta ni ganancia ocasional) | Si no vendes más del 3% de las acciones en circulación de esa sociedad en el año (Art. 36-1 ET). Para un inversionista normal, casi siempre se cumple. |
| **eToro / extranjero** | Ganancia ocasional al 15% | Si se mantiene ≥ 2 años y se considera activo fijo. Si se vende antes de 2 años, puede ser renta ordinaria (hasta 39%). |

## Impacto neto al retiro (incluyendo impuestos)

| Escenario | Valor final | Impuesto sobre ganancias | Valor neto final |
|-----------|-------------|---------------------------|------------------|
| FPV (3.5% comisión) | aprox. $476 millones | $0 (si cumple condiciones) | **aprox. $476 millones** |
| eToro (0.05% comisión) | aprox. $665 millones | aprox. $73 millones (15%) | **aprox. $592 millones** |
| BVC (si aplica Art. 36-1) | aprox. $665 millones | $0 | **aprox. $665 millones** |

Incluso pagando el 15% de ganancia ocasional en eToro, el resultado neto (aprox. $592 millones) sigue siendo alrededor del **24% superior** al FPV (aprox. $476 millones). La diferencia es de unos **$116 millones** a favor de la autoinversión de bajo costo.

## Resumen práctico

- La comisión del **3.5%** del FPV sigue siendo el factor que más destruye el resultado a largo plazo.
- El beneficio de no pagar ganancia ocasional en el FPV (o en la BVC) no alcanza a compensar ese costo de comisión tan alto.
- Entre eToro (con 15%) y BVC (potencialmente exento), la BVC es más eficiente tributariamente para acciones colombianas, siempre que no superes el límite del 3%.
- Cuando el cupo de renta exenta ya está lleno, el beneficio adicional de meter más dinero al FPV es limitado, mientras que el costo de la comisión es permanente.
- Además, existe un **costo de oportunidad** por el lockup: para conservar la exención debes mantener el capital al menos 10 años (o cumplir condiciones específicas). Si necesitas liquidez antes, pierdes el beneficio tributario y puedes enfrentar retención. En una inversión propia (BVC o ETFs) puedes rebalancear o retirar sin esa restricción.

**Conclusión**: incluso considerando el 15% de ganancia ocasional en eToro, sigue siendo más conveniente invertir por tu cuenta en ETFs de bajo costo que pagar 3.5% de comisión en un FPV, a menos que la comisión real de tu fondo sea significativamente más baja (idealmente ≤ 1.5–2%).

## Cómo usar

1. Clona el repositorio.
2. Abre `simulacion_comisiones.ipynb` en Jupyter o Google Colab.
3. Ejecuta las celdas para ver los gráficos y tablas.

---

*Este es un ejemplo ilustrativo. Los resultados dependen de la rentabilidad real, las comisiones exactas de cada fondo y la situación tributaria particular de cada persona.*
