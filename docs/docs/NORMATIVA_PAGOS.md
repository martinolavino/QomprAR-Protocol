# 📚 Marco Normativo: Pagos en Argentina

Para el desarrollo de QomprAR, el equipo debe alinearse con las siguientes normativas del Banco Central de la República Argentina (BCRA):

### 1. Transferencias 3.0 (Interoperabilidad)
- **Concepto:** Todo QR debe ser aceptado por todas las billeteras.
- **Protocolo:** Uso de las interfaces de **COELSA** para el movimiento de fondos entre cuentas (CBU/CVU).
- **Plazos de Acreditación:** Los pagos con transferencia deben ser **irreversibles y de acreditación inmediata** para el comercio.

### 2. PSP (Proveedores de Servicios de Pago)
- QomprAR opera bajo la figura de **PSPCP** (Proveedor de Servicios de Pago que ofrece Cuentas de Pago).
- Se debe garantizar la segregación de fondos: el dinero de los usuarios debe estar en una cuenta "a la vista" en un banco comercial, separada de los fondos operativos de la plataforma.

### 3. Estándares de Seguridad
- Cumplimiento con estándares de cifrado para el manejo de datos de tarjetas (si se usa Soft-POS) según normas **PCI-DSS**.
- Autenticación de dos factores (2FA) para movimientos de fondos salientes.
