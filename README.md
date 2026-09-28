# SauceDemo UI & Network Resiliency - Manual Testing Project

## Descripción
Este proyecto de **QA Manual** enfocado en el aseguramiento de la calidad (Quality Assurance) fue ejecutado sobre la aplicacion **SauceDemo (Swag Labs)**. El objetivo principal fue auditar el ciclo completo de autenticación y control de accesos del módulo de Login. 

A diferencia de un testing superficial, este análisis abarcó validaciones de interfaz de usuario (UI), lógica de negocio, control de sesiones, **auditoría de tráfico de red en el cliente (Client-Side Network Inspection)** y **resiliencia del sistema ante cortes de conectividad**.

---

## Aplicación y Entorno Bajo Prueba
*   **Plataforma:** SauceDemo (Swag Labs)
*   **URL Oficial:** [https://saucedemo.com](https://saucedemo.com)
*   **Módulo Auditado:** Formulario de Autenticación y Gestión de Sesiones (Login / Logout).
*   **Ambiente de Pruebas:** Producción (Pruebas Web de Caja Negra).

---

## Tipos de Testing Aplicados
Para maximizar la cobertura del módulo se aplicaron las siguientes disciplinas de prueba:
*   **Functional Testing:** Verificación de las reglas de negocio del login.
*   **Positive & Negative Testing:** Validación de flujos felices y manejo controlado de excepciones con datos erróneos.
*   **UI/UX Validation Testing:** Inspección de estilos visuales de error, bordes dinámicos e iconografía de alerta.
*   **Security & Session Testing:** Análisis de persistencia de tokens de usuario, rutas protegidas y destrucción de sesiones en memoria caché.
*   **Non-Functional Resiliency Testing:** Simulación de fallos de entorno (Modo Offline) para evaluar la estabilidad de la arquitectura SPA.

---

## Alcance e Ingeniería de Pruebas
El plan de pruebas se dividió estratégicamente en **8 Escenarios de Prueba (Test Scenarios)** generales, de los cuales se desprendieron **20 Casos de Prueba (Test Cases)**:

*   **TS-001:** Validación de inicio de sesión con credenciales válidas y carga del catálogo.
*   **TS-002:** Verificación de campos obligatorios y prioridad de alertas en el formulario.
*   **TS-003:** Control de accesos ante credenciales inválidas (Casos Negativos).
*   **TS-004:** Reglas de campos de texto (Enmascaramiento de contraseñas y sanitización de espacios en blanco).
*   **TS-005:** Comportamiento lógico del disparador de autenticación (Interacciones rápidas y eventos de teclado).
*   **TS-006:** Seguridad de la sesión (Bloqueo de URLs protegidas sin autenticación activa y persistencia mediante F5).
*   **TS-007:** Funcionalidad de cierre de sesión (Logout) y deshabilitación del botón "Atrás" del navegador.
*   **TS-008:** Pruebas avanzadas de resiliencia de red y auditoría de payloads de tráfico local.

---

## Herramientas Utilizadas
*   **Jira** 
*   **Microsoft Excel** 
*   **Sauce Demo** 
*   **Google Chrome DevTools**
*   **Lightshot / Snipping Tool** 

---

## Resultados de la Ejecución


| Métrica | Valor | Estado |
| :--- | :---: | :---: |
| **Casos de Prueba Diseñados** | 20 | 100% |
| **Casos de Prueba Ejecutados** | 20 | 100% |
| **Casos Exitosos (PASS)** | 20 | Exitoso |
| **Casos Fallidos (FAIL)** | 0 | Limpio |
| **Bugs Críticos Detectados** | 0 | N/A |

### Conclusión del Análisis:
Se completó con éxito el ciclo de aseguramiento de calidad sobre el módulo de autenticación de SauceDemo, logrando una cobertura del 100% en los escenarios críticos de negocio.  A través de la ejecución de los 20 casos de prueba, se validó que la plataforma responde de forma robusta y segura tanto en sus flujos felices como en el manejo controlado de errores y excepciones de usuario. 

La integración de herramientas de desarrollador permitió comprobar que el sistema gestiona la persistencia de sesiones y la estabilidad de la interfaz bajo estándares óptimos, garantizando una experiencia de usuario fluida, segura y altamente confiable.


