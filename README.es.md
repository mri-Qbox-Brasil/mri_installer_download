# MRI Installer - Distribución Oficial 🚀

Leer en: [🇧🇷 Português](README.md) | [🇺🇸 English](README.en.md)

El **MRI Installer** es la puerta de entrada al ecosistema **MRI Qbox Brasil**. Una herramienta profesional, resiliente y segura para automatizar la instalación de su servidor FiveM.

[![GitHub release (latest by date)](https://img.shields.io/github/v/release/mri-Qbox-Brasil/mri_installer_download?style=for-the-badge&color=7289da)](https://github.com/mri-Qbox-Brasil/mri_installer_download/releases/latest)
[![Security - VirusTotal Verified](https://img.shields.io/badge/Security-VirusTotal%20Scan-blue?style=for-the-badge&logo=virustotal)](https://github.com/mri-Qbox-Brasil/mri_installer_download/releases/latest)

---

## ✨ ¿Por qué usar MRI Installer?

A diferencia de los instaladores comunes, MRI fue construido centrándose en la **estabilidad** y la **seguridad**:

- 🛡️ **Seguridad Verificada**: Cada versión enviada a este repositorio es escaneada automáticamente por **VirusTotal**. El enlace del informe está disponible en cada release.
- 💾 **Instalación Resiliente (Resume)**: ¿Se cayó el internet o se apagó la PC? El instalador detecta dónde se detuvo y reanuda el progreso automáticamente, sin corromper archivos.
- 🗄️ **Base de Datos Automática**: ¿No tiene MariaDB instalado? El software se encarga de eso por usted en segundo plano, con resiliencia contra bloqueos de Windows (UAC). ¿Ya tiene una base de datos? Apúntela a cualquier host/puerto existente y vea la contraseña mientras la configura.
- 👑 **txAdmin Personalizado**: El instalador configura automáticamente el nombre de su servidor y el idioma en el panel administrativo.
- 🌎 **Soporte Multilingüe**: Interfaz intuitiva y soporte completo para español, portugués e inglés.
- 🐧 **Soporte para Linux**: Binario nativo para servidores Linux con instalador de terminal interactivo o totalmente automatizado mediante flags.

## 🚀 Cómo Empezar

### Windows (interfaz gráfica)

1. Vaya a la pestaña [**Releases**](https://github.com/mri-Qbox-Brasil/mri_installer_download/releases/latest).
2. Descargue el archivo `mri_installer.exe`.
3. Ejecute el instalador y siga los 7 pasos guiados (Ambiente, Motor, Receta, Resumen, Deploy, Configuración y Dashboard).

### Linux (terminal / servidor headless)

1. Vaya a la pestaña [**Releases**](https://github.com/mri-Qbox-Brasil/mri_installer_download/releases/latest).
2. Descargue el archivo `mri_installer_linux`.
3. Otorgue permiso de ejecución y ejecute:

```bash
chmod +x mri_installer_linux

# Modo interactivo (recomendado para principiantes)
./mri_installer_linux

# Modo no interactivo (flags completas)
./mri_installer_linux \
  --install-path /opt/fivem/mri_qbox \
  --server-name "Mi Servidor" \
  --license-key "cfxk_..." \
  --db-pass "contraseña" \
  --install-mariadb

# Subcomandos, para servidores ya instalados
./mri_installer_linux --login
./mri_installer_linux --update-artifacts --install-path /opt/fivem/mri_qbox
./mri_installer_linux --backup --install-path /opt/fivem/mri_qbox
./mri_installer_linux --list-resources --install-path /opt/fivem/mri_qbox
```

> [!NOTE]
> En modo interactivo, el instalador muestra un **código de autorización** de 8 caracteres. Autorízalo ejecutando `/liberar <código>` en nuestro Discord **o** abriendo el enlace mostrado — sin necesidad de navegador en el servidor.

> [!TIP]
> **Consejo de Seguridad**: Asegúrese siempre de descargar el ejecutable de este repositorio oficial de la organización **MRI Qbox Brasil**.

## 🛡️ Transparencia y Seguridad

Nos tomamos en serio la seguridad de nuestra comunidad. Por eso, integramos nuestro pipeline de publicación con la API de **VirusTotal**.

Puede encontrar el sello de seguridad y el enlace al informe técnico completo en la descripción de cada versión lanzada.

El instalador tampoco **incluye ninguna credencial**: la validación de acceso y la descarga de recetas ocurren en nuestros servidores, por lo que inspeccionar el binario no revela claves ni secretos.

---

Desarrollado con ❤️ por el equipo [MRI QBOX BRASIL](https://github.com/mri-qbox-brasil)
