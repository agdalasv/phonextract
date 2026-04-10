# 📞 PhoneXtract - Number Intelligence Tool

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.8+-blue?style=flat&logo=python" alt="Python">
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat" alt="License">
  <img src="https://img.shields.io/badge/Platform-Linux%20%7C%20Windows%20%7C-Android-purple?style=flat" alt="Platform">
</p>

---

## 📌 Descripción

PhoneXtract es una herramienta OSINT (Open Source Intelligence) escrita en Python para obtener información básica sobre cualquier número telefónico a nivel mundial. Ideal para propósitos educativos e investigadores de seguridad.

> ⚠️ **Solo para uso educativo e investigativo.** El autor no se hace responsable del uso indebido de esta herramienta.

---

## ⚙️ Características

- 📍 **Ubicación** - Obtiene la ubicación (estado/región) del número telefónico
- 📡 **Operador** - Detecta el nombre del operador (Airtel, Jio, AT&T, Vodafone, etc.)
- 📞 **Tipo de teléfono** - Identifica si es Móvil, Línea Fija, VoIP
- 🕰️ **Zona horaria** - Zona horaria del número
- 🌐 **Formatos** - Formatos Nacional e Internacional
- ✅ **Validación** - Verifica si el número es válido
- 🔠 **Análisis de prefijos** - Código de área y prefijo
- 🏙️ **Ciudad/Estado/Región** - Ubicación aproximada mediante mapeo de prefijos
- 📱 **Verificación WhatsApp** - Verifica si el número está registrado en WhatsApp
- 🔍 **Redes Sociales** - Busca el número en Facebook, Instagram, Telegram, LinkedIn
- 🚫 **Reportes Spam** - Verifica en bases de datos públicas de spam

---

## 🌍 Soporte Internacional

PhoneXtract soporta números telefónicos de **todos los países** usando la librería `phonenumbers`.

**Regiones soportadas:**
| Región | Ejemplos |
|--------|----------|
| 🇮🇳 Asia del Sur | India, Paquistán, Bangladesh, Nepal, Sri Lanka |
| 🇺🇸 América del Norte | USA, Canadá, México |
| 🇬🇧 Europa | UK, Alemania, Francia, Italia, España, Rusia |
| 🇦🇪 Medio Oriente | UAE, Arabia Saudita, Qatar, Kuwait |
| 🇨🇳 Asia Oriental | China, Japón, Corea del Sur |
| 🇧🇷 América del Sur | Brasil, Argentina, Colombia |
| 🇿🇦 África | Sudáfrica, Nigeria, Kenia, Egipto |
| 🇦🇸 Oceanía | Australia, Nueva Zelanda |

> ✅ **Siempre usa el formato internacional completo con código de país.**
> Ejemplo: `+14155552671` (USA), `+447911123456` (UK), `+919876543210` (India)

---

## ⚠️ Disclaimer de Precisión

> **La información mostrada por PhoneXtract NO siempre es 100% precisa.**

- Los datos del operador pueden estar desactualizados (portación de números)
- La ubicación se basa en prefijos, no en GPS real
- La precisión varía por país (mayor para India)
- La verificación de WhatsApp es solo esfuerzo máximo

---

## 📲 Instalación

### 🐧 Arch Linux

```bash
# Actualizar sistema
sudo pacman -Syu

# Instalar dependencias
sudo pacman -S python python-pip git

# Clonar repositorio
git clone https://github.com/thakur2309/phonextract.git
cd phonextract

# Crear entorno virtual
python -m venv venv

# Activar entorno virtual
source venv/bin/activate

# Instalar dependencias
pip install -r requirements.txt

# Ejecutar
python phonextract.py
```

**Para ejecutar nuevamente:**
```bash
cd phonextract
source venv/bin/activate
python phonextract.py
```

---

### 🐧 Ubuntu / Debian

```bash
# Actualizar sistema
sudo apt update && sudo apt upgrade -y

# Instalar dependencias
sudo apt install python3 python3-pip python3-venv git -y

# Clonar repositorio
git clone https://github.com/thakur2309/phonextract.git
cd phonextract

# Crear entorno virtual
python3 -m venv venv

# Activar entorno virtual
source venv/bin/activate

# Instalar dependencias
pip install -r requirements.txt

# Ejecutar
python3 phonextract.py
```

**Para ejecutar nuevamente:**
```bash
cd phonextract
source venv/bin/activate
python3 phonextract.py
```

---

### 🎩 Fedora

```bash
# Actualizar sistema
sudo dnf update -y

# Instalar dependencias
sudo dnf install python3 python3-pip git -y

# Clonar repositorio
git clone https://github.com/thakur2309/phonextract.git
cd phonextract

# Crear entorno virtual
python3 -m venv venv

# Activar entorno virtual
source venv/bin/activate

# Instalar dependencias
pip install -r requirements.txt

# Ejecutar
python3 phonextract.py
```

**Para ejecutar nuevamente:**
```bash
cd phonextract
source venv/bin/activate
python3 phonextract.py
```

---

### 📱 Termux (Android)

```bash
# Actualizar sistema
pkg update && pkg upgrade -y

# Instalar dependencias
pkg install git python -y

# Clonar repositorio
git clone https://github.com/thakur2309/phonextract.git
cd phonextract

# Instalar dependencias
pip install -r requirements.txt

# Ejecutar
python phonextract.py
```

---

### 🪟 Windows

```bash
# Requirements
# - Python 3.x - Descargar de python.org
# - Git - Descargar de git-scm.com

# En CMD o PowerShell
git clone https://github.com/thakur2309/phonextract.git
cd phonextract
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
python phonextract.py
```

---

## 🚀 Uso

1. Ejecuta el script: `python phonextract.py` (o `python3` en Linux)
2. Ingresa el número telefónico con código de país (ej: +50512345678)
3. La herramienta mostrará información detallada del número

---

## 📂 Estructura del Proyecto

```
phonextract/
├── phonextract.py      # Script principal
├── requirements.txt    # Dependencias
├── README.md           # Este archivo
├── LICENSE             # Licencia MIT
└── venv/               # Entorno virtual (no incluido en Git)
```

---

## 📋 Requisitos

- Python 3.8+
- phonenumbers
- colorama
- requests

---

## 🔧 Configuración de GitHub Pages

El sitio web está disponible en: **https://TU_USUARIO.github.io/phonextract/**

Para configurar GitHub Pages:
1. Ve a Settings > Pages
2. En "Source", selecciona "main" branch
3. El sitio se publicará automáticamente

---

## 📱 Redes del Creador

<p align="center">
  <a href="https://youtube.com/@firewallbreaker09">
    <img src="https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white" alt="YouTube">
  </a>
  <a href="https://github.com/thakur2309">
    <img src="https://img.shields.io/badge/GitHub-000000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub">
  </a>
  <a href="https://wa.me/yournumber">
    <img src="https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white" alt="WhatsApp">
  </a>
</p>

---

## 📄 Licencia

Este proyecto está bajo la Licencia MIT. Consulta el archivo `LICENSE` para más detalles.

---

<p align="center">⭐ Si te fue útil, por favor dale una estrella al repositorio</p>
<p align="center">Hecho con ❤️ por Agdala | TikTok: @agdalasv</p>