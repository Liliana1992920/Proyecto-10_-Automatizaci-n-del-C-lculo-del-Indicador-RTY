# Informe Final del Proyecto: Automatización del Cálculo del Indicador RTY

## **Descripción del Proyecto**
Este proyecto se enfocó en automatizar el cálculo del indicador **RTY (Rolled Throughput Yield)** mediante pruebas exclusivas en el back-end. Las validaciones se realizaron directamente en la base de datos del sistema en un ambiente de QA, utilizando datos insertados manualmente mediante consultas SQL.

---

## **Objetivos del Proyecto**
1. Validar el cálculo automatizado del indicador RTY en la base de datos.
2. Insertar datos representativos para pruebas, simulando escenarios reales y extremos.
3. Verificar la consistencia y precisión de los resultados generados por el sistema.
4. Identificar y documentar errores en caso de discrepancias.

---

## **Metodología**
1. **Ambiente de Pruebas:**
   - **Entorno:** Ambiente de QA.
   - **Base de Datos:** SQL Server Management Studio (SSMS).

2. **Preparación de Datos:**
   - Inserción de registros de prueba en las tablas relacionadas con el cálculo del RTY.

3. **Ejecución de Pruebas:**
   - Validación del cálculo mediante consultas SQL.
   - Comparación de resultados obtenidos frente a los resultados esperados.

4. **Reporte de Errores:**
   - Documentación de errores encontrados en **Jira**.

---

### **2. Validación del Cálculo de RTY**

#### **Fórmula Utilizada**
La fórmula para calcular el indicador **RTY (Rolled Throughput Yield)** es:

\[
RTY = \prod_{i=1}^{n} \frac{\text{TotalOutput}_i}{\text{TotalInput}_i}
\]
# Conclusiones y Recomendaciones: Automatización del Cálculo del Indicador RTY

## **Conclusiones**
1. **Cálculo Preciso:** 
   - El sistema calcula correctamente el indicador RTY utilizando la fórmula estándar.
   - Los resultados obtenidos para casos normales y extremos fueron precisos y consistentes.

2. **Estabilidad:**
   - El sistema maneja adecuadamente excepciones en escenarios donde los datos son inconsistentes o presentan errores comunes (e.g., `TotalInput = 0` o `TotalOutput > TotalInput`).

3. **Preparación para Producción:**
   - El sistema demostró estar listo para implementarse en un entorno de producción, dado que no se identificaron errores críticos durante las pruebas en el ambiente de QA.

---

## **Recomendaciones**

1. **Automatización de Pruebas:**
   - Implementar pruebas automáticas para verificar el cálculo del RTY con diferentes combinaciones de datos y escenarios extremos.
   - Usar herramientas como **Selenium**, **Postman** o scripts personalizados para validaciones continuas.

2. **Validación Continua:**
   - Realizar auditorías periódicas de los cálculos de RTY con datos en tiempo real para garantizar que los resultados sigan siendo precisos después de actualizaciones del sistema.

3. **Mejorar la Documentación:**
   - Documentar las fórmulas utilizadas, los supuestos de cálculo, y los posibles casos de error para referencia futura.
   - Crear guías detalladas para desarrolladores y usuarios finales sobre cómo interpretar y usar los resultados de RTY.

4. **Optimización del Sistema:**
   - Evaluar el impacto del volumen de datos en el tiempo de procesamiento y, si es necesario, optimizar las consultas SQL utilizadas para cálculos en grandes conjuntos de datos.

---

**Equipo QA**  
 


