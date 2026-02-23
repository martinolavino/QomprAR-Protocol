# Visión Técnica y Hoja de Ruta - QomprAR

Este documento detalla la arquitectura lógica y las fases de desarrollo de QomprAR. El objetivo es construir una infraestructura digital soberana que sea potente en su ejecución pero extremadamente simple para el usuario final.

## 🛠️ Principios de Desarrollo
1. **Simplicidad Radical:** La tecnología debe ser invisible. Si el "hombre de a pie" no entiende la interfaz, el diseño ha fallado.
2. **Soberanía del Usuario:** El usuario es dueño de sus datos y de su reputación.
3. **Privacidad Modular:** Las integraciones con entes reguladores (como AFIP) son estrictamente opcionales.

---

## 🗺️ Hoja de Ruta de Producto

### Paso 1: Billetera Digital y Facturador Opcional
El núcleo del ecosistema. Una billetera para gestionar **Pesos Digitales (ARST)** con paridad 1:1.
* **Rendimientos Diarios:** Distribución automática de intereses generados por la reserva de liquidez.
* **Facturador AFIP (Módulo Opcional):** Integración con Web Services de AFIP para profesionales que requieran emitir comprobantes. El usuario decide si activa esta función o si opera de forma privada.
* **Tecnología:** Account Abstraction para eliminar la fricción de las llaves privadas.

### Paso 2: Plataforma de Venta (Marketplace)
Extensión de la billetera hacia un catálogo de productos y servicios locales.
* **Comisiones Mínimas:** Reducción drástica comparado con plataformas tradicionales (~2% vs 15-30%).
* **Migración de Reputación:** Herramientas para importar calificaciones desde sistemas externos (ML, Uber, etc.).

### Paso 3: Logística de Movilidad Integral
