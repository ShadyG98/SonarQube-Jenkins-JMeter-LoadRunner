# 🧪 QA & Testing Tools Overview

Resumen completo de las principales herramientas de **QA y testing**, sus usos, diferencias y recomendaciones.

---

## 🔹 Herramientas Principales

| Herramienta   | Tipo                             | Uso principal                        | Detalles y ventajas |
|---------------|---------------------------------|-------------------------------------|-------------------|
| **SonarQube** | Análisis de código estático      | Evaluar la calidad del código, detectar bugs y vulnerabilidades. | Permite medir deuda técnica, duplicaciones, cobertura de pruebas unitarias y complejidad del código. Integrable con pipelines CI/CD. |
| **Jenkins**   | CI/CD y automatización           | Automatizar builds, pruebas y despliegues. | Compatible con múltiples lenguajes y herramientas. Permite pipelines declarativos o freestyle. Muy usado en DevOps. |
| **JMeter**    | Pruebas de carga y performance   | Simular carga de usuarios, medir rendimiento y estabilidad. | Ideal para pruebas de estrés, rendimiento y benchmarking de APIs o aplicaciones web. Soporta múltiples protocolos: HTTP, SOAP, JDBC, etc. |
| **LoadRunner**| Pruebas de rendimiento           | Evaluar capacidad y escalabilidad de sistemas críticos. | Permite modelar escenarios complejos de carga, medir tiempos de respuesta y generar reportes detallados. Compatible con aplicaciones web, móviles y mainframes. |

---

## 🔹 Diferencias Clave

- **SonarQube vs Jenkins:** SonarQube analiza el código, mientras que Jenkins ejecuta pipelines completos de integración y despliegue.  
- **JMeter vs LoadRunner:** Ambos miden rendimiento, pero JMeter es open-source y más flexible para pruebas simples, mientras LoadRunner es pago, con más soporte y escenarios complejos.  
- **Integración CI/CD:** SonarQube y JMeter/LoadRunner pueden integrarse con Jenkins para reportes y automatización.  

---

## 🔹 Pipeline conceptual

Se recomienda un flujo básico de CI/CD con QA:

1. **Commit de código** → 2. **Build y Unit Tests (Jenkins)** → 3. **Análisis de calidad (SonarQube)** → 4. **Pruebas de rendimiento (JMeter/LoadRunner)** → 5. **Reporte y despliegue**

> Esta estructura permite detectar errores y problemas de performance antes de producción.

---

## 🔹 Recomendaciones de Uso

1. **SonarQube:** Integrar en el pipeline para medir métricas de calidad en cada commit.  
2. **Jenkins:** Automatizar build, test y despliegue para minimizar errores manuales.  
3. **JMeter:** Ejecutar pruebas de carga periódicas para detectar cuellos de botella.  
4. **LoadRunner:** Usar para pruebas críticas de alto impacto y simulaciones de tráfico realista.  

---

## 🔹 Referencias

- [SonarQube](https://www.sonarqube.org/)  
- [Jenkins](https://www.jenkins.io/)  
- [JMeter](https://jmeter.apache.org/)  
- [LoadRunner](https://docs.microfocus.com/doc/123/9.60/configrunloadtest)  

---

## 🔹 Contribuciones

Se aceptan PRs para agregar nuevas herramientas o mejorar descripciones.

---

## 🔹 Licencia

MIT License © 2025
