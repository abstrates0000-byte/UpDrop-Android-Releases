# UpDrop Android — APKs oficiales

Repositorio público **solo para APKs firmadas**. El código fuente de UpDrop sigue privado.

## Versión más reciente: 0.2.1

**[Descargar UpDrop Android 0.2.1](https://github.com/abstrates0000-byte/UpDrop-Android-Releases/releases/download/v0.2.1/UpDrop-Android.apk)**

- Corrección de compatibilidad de cadena de certificados TLS y diagnósticos detallados en la app.
- Mismo paquete y certificado de firma Android que 0.1.0 y 0.2.0: **actualiza sin desinstalar**.
- En Will27: **cierra el receptor anterior** con Ctrl+C, abre nuevamente **UpDrop - Recibir Android** y **escanea un QR nuevo** porque cambió la CA local (la CA anterior se conserva sin sobrescribirla).
- Piloto de envío Android → Windows por LAN: TLS 1.3, huella verificada, autorización por archivo en la consola Windows, SHA-256. Límite 256 MiB, sin reanudación ni envío Windows → Android.
- SHA-256 de la APK: `d68462bc52c9585a1f2b91cc1cc635f5ed5192ed6f41a0e11da487f884d15b36`.
- **Todavía falta comprobar la transferencia en el Motorola real.** Si vuelve a aparecer `CertificateUnknown`, copia el error **detallado que muestra Android** (sin compartir el QR ni PAIR_TOKEN). No desactives TLS.

[Historial de versiones y notas](https://github.com/abstrates0000-byte/UpDrop-Android-Releases/releases).

Al pulsar **Buscar actualización**, UpDrop consulta GitHub Releases, compara versión, SHA-256, paquete y firma, y pide a Android la instalación con confirmación del usuario. No contiene tokens personales de GitHub.
