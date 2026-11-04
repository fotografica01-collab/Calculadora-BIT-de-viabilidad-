# Calculadora de Viabilidad BIT

Proyecto de herramienta interna de BIT Market, dentro de
Atlas Core, para apoyar la evaluación económica de productos
antes de realizar una compra y preparar su comercialización.

## Objetivo

Organizar los costos de adquisición, logística y venta para
estimar cuánto cuesta cada unidad, qué resultado económico
podría generar y bajo qué condiciones sería viable comprarla.

La herramienta apoyará la toma de decisiones mediante
cálculos verificables y escenarios comparables.

## Contexto de operación

BIT Market adquiere productos mediante proveedores y servicios
de terceros para la gestión logística y de importación.

Los cálculos deberán representar esta modalidad de operación
e identificar qué conceptos están incluidos en cada factura
o cotización, para evitar contabilizarlos dos veces.

## Funciones previstas

- Identificar el producto, proveedor y CDI, cuando corresponda.
- Registrar cantidades y precios de compra.
- Diferenciar valores en dólares y pesos colombianos.
- Registrar la tasa de cambio utilizada.
- Incluir comisiones y gastos adicionales aplicables.
- Calcular el volumen de la mercancía en metros cúbicos.
- Incorporar tarifas logísticas y transporte nacional.
- Calcular el costo total y el costo por unidad.
- Registrar un precio de venta propuesto.
- Diferenciar margen sobre ventas y recargo sobre costo.
- Estimar la contribución después de los costos variables de venta.
- Calcular el punto de equilibrio cuando existan datos suficientes.
- Comparar escenarios de costos, precios y cantidades.

## Datos y trazabilidad

Cada evaluación deberá identificar, según corresponda:

- Producto y código interno.
- CDI o referencia de compra.
- Fecha de elaboración.
- Fuentes de los valores utilizados.
- Moneda y tasa de cambio.
- Supuestos del escenario.
- Información pendiente de confirmar.
- Versión y estado de la evaluación.

Los datos faltantes deberán mostrarse como pendientes.
No deberán convertirse automáticamente en cero ni presentarse
como información confirmada.

## Reglas de cálculo

Las fórmulas, tarifas y criterios deberán documentarse
y validarse antes de utilizar la herramienta para decisiones
reales de compra.

Se deberá evitar la duplicación de gastos incluidos en
facturas, cotizaciones o servicios de terceros.

Los resultados deberán distinguir entre cálculos basados en
datos confirmados y simulaciones basadas en supuestos.

La evaluación económica será un insumo para la decisión.
La autorización de compra también dependerá de la evaluación
comercial, técnica y regulatoria correspondiente.

## Relación con Atlas Core

La herramienta se vinculará principalmente con:

- M01: Radar y selección de productos.
- M02: Proveedores y negociación.
- M03: Compras, logística y costos.
- M05: Construcción de ofertas.
- M09: Analítica y resultados.

Se prevé facilitar su acceso desde el panel central de Atlas Core.
La forma de integración se definirá durante el desarrollo.

## Desarrollo por etapas

1. Definir los datos de entrada y las fórmulas.
2. Construir una primera calculadora funcional.
3. Comprobar los resultados con casos de prueba.
4. Validar su funcionamiento con un caso real.
5. Incorporar almacenamiento y exportación de evaluaciones.
6. Publicar la herramienta e integrarla al panel central.

## Estado actual

Proyecto en preparación.

Este documento describe el alcance previsto.
Las funciones se implementarán y verificarán progresivamente.
