<div align="center">

<img src="https://img.shields.io/badge/FiveM-Script-FF6B6B?style=for-the-badge&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAAOCAYAAAAfSC3RAAAACXBIWXMAAAsTAAALEwEAmpwYAAAA" />

# 🚗 max-speed

**Universal Vehicle Speed Limiter for FiveM**

[![Version](https://img.shields.io/badge/version-1.0.0-blue?style=flat-square)](https://github.com)
[![Framework](https://img.shields.io/badge/framework-Standalone%20%7C%20ESX%20%7C%20QBCore%20%7C%20QBX-green?style=flat-square)](https://github.com)
[![FiveM](https://img.shields.io/badge/FiveM-Compatible-red?style=flat-square)](https://fivem.net)
[![License](https://img.shields.io/badge/license-MIT-yellow?style=flat-square)](LICENSE)

---

*🌍 [العربية](#-العربية) · [English](#-english) · [Français](#-français) · [Español](#-español) · [Deutsch](#-deutsch) · [Português](#-português)*

</div>

---

## 🇲🇦 العربية

### 📖 وصف السكريبت

**max-speed** هو ريسورس خفيف ومحترف لـ FiveM يضع حداً أقصى لسرعة جميع السيارات.  
فاش توصل السيارة للحد — تبقى **ستابل** بالضبط بلا كروز أوتوماتيك ولا أي تأثير جانبي.

### ✅ المميزات

- 🔒 حد أقصى قابل للتعديل (افتراضي: **290 كم/ساعة**)
- ⚡ خفيف جداً — يشتغل في لوب كل فريم
- 🎯 يطبّق فقط على السائق مش الراكبين
- 🔄 يعمل مع جميع الفريموركات بدون تعديل
- 🛠️ سهل التثبيت — ملف واحد للإعداد

### 📦 التثبيت

```
1. حط مجلد max-speed في resources ديالك
2. زيد في server.cfg:
       ensure max-speed
3. عيّط السيرفر
```

### ⚙️ الإعداد

في ملف `client.lua` السطر 8:
```lua
local MAX_SPEED_KMH = 290.0   -- ← غيّر هنا
```

### 🤝 التوافق مع الفريموركات

| الفريمورك | متوافق | ملاحظات |
|-----------|--------|---------|
| **Standalone** | ✅ | يشتغل مباشرة |
| **ESX** | ✅ | ما محتاجش أي تعديل |
| **QBCore** | ✅ | ما محتاجش أي تعديل |
| **QBX** | ✅ | ما محتاجش أي تعديل |

---

## 🇬🇧 English

### 📖 Description

**max-speed** is a lightweight and plug-and-play FiveM resource that enforces a maximum speed cap on all vehicles.  
When a vehicle reaches the configured speed — it stays **stable** at that exact limit, with no auto-cruise or side effects.

### ✅ Features

- 🔒 Configurable max speed (default: **290 km/h**)
- ⚡ Extremely lightweight — runs each frame efficiently
- 🎯 Applies only to the driver, not passengers
- 🔄 Works with all frameworks without any modification
- 🛠️ Easy install — single config variable

### 📦 Installation

```
1. Drop the max-speed folder into your resources directory
2. Add to server.cfg:
       ensure max-speed
3. Restart your server
```

### ⚙️ Configuration

In `client.lua` line 8:
```lua
local MAX_SPEED_KMH = 290.0   -- Change this value
```

| Value | Speed |
|-------|-------|
| `290.0` | 290 km/h (default) |
| `250.0` | 250 km/h |
| `320.0` | 320 km/h |

### 🤝 Framework Compatibility

| Framework | Supported | Notes |
|-----------|-----------|-------|
| **Standalone** | ✅ | Works out of the box |
| **ESX** | ✅ | No modification needed |
| **QBCore** | ✅ | No modification needed |
| **QBX** | ✅ | No modification needed |

### 🔧 How It Works

The script runs a client-side loop every frame. It checks if the local player is the driver of a vehicle. If the vehicle speed reaches or exceeds the configured maximum, `SetEntityMaxSpeed` is called to enforce the cap smoothly. Below the cap, the vehicle behaves completely normally.

---

## 🇫🇷 Français

### 📖 Description

**max-speed** est un resource FiveM léger et universel qui impose une vitesse maximale à tous les véhicules.  
Quand un véhicule atteint la limite configurée — il reste **stable** à cette vitesse exacte, sans pilote automatique ni effets secondaires.

### ✅ Fonctionnalités

- 🔒 Vitesse max configurable (par défaut : **290 km/h**)
- ⚡ Ultra-léger — boucle optimisée par frame
- 🎯 S'applique uniquement au conducteur, pas aux passagers
- 🔄 Compatible avec tous les frameworks sans modification
- 🛠️ Installation simple — une seule variable à configurer

### 📦 Installation

```
1. Placez le dossier max-speed dans votre répertoire resources
2. Ajoutez dans server.cfg :
       ensure max-speed
3. Redémarrez votre serveur
```

### ⚙️ Configuration

Dans `client.lua` ligne 8 :
```lua
local MAX_SPEED_KMH = 290.0   -- Modifiez cette valeur
```

### 🤝 Compatibilité

| Framework | Supporté | Notes |
|-----------|----------|-------|
| **Standalone** | ✅ | Fonctionne immédiatement |
| **ESX** | ✅ | Aucune modification requise |
| **QBCore** | ✅ | Aucune modification requise |
| **QBX** | ✅ | Aucune modification requise |

---

## 🇪🇸 Español

### 📖 Descripción

**max-speed** es un resource ligero y universal para FiveM que establece una velocidad máxima para todos los vehículos.  
Cuando un vehículo alcanza el límite — se mantiene **estable** en esa velocidad exacta, sin piloto automático ni efectos secundarios.

### ✅ Características

- 🔒 Velocidad máxima configurable (por defecto: **290 km/h**)
- ⚡ Muy ligero — bucle eficiente por frame
- 🎯 Solo aplica al conductor, no a los pasajeros
- 🔄 Compatible con todos los frameworks sin modificación
- 🛠️ Instalación sencilla — una sola variable

### 📦 Instalación

```
1. Coloca la carpeta max-speed en tu directorio resources
2. Añade en server.cfg:
       ensure max-speed
3. Reinicia tu servidor
```

### ⚙️ Configuración

En `client.lua` línea 8:
```lua
local MAX_SPEED_KMH = 290.0   -- Cambia este valor
```

---

## 🇩🇪 Deutsch

### 📖 Beschreibung

**max-speed** ist ein leichtes und universelles FiveM-Resource, das eine Höchstgeschwindigkeit für alle Fahrzeuge erzwingt.  
Wenn ein Fahrzeug das Limit erreicht — bleibt es **stabil** bei genau dieser Geschwindigkeit, ohne Tempomat oder Nebeneffekte.

### ✅ Funktionen

- 🔒 Konfigurierbare Höchstgeschwindigkeit (Standard: **290 km/h**)
- ⚡ Sehr leichtgewichtig — effiziente Frame-Schleife
- 🎯 Gilt nur für den Fahrer, nicht für Mitfahrer
- 🔄 Kompatibel mit allen Frameworks ohne Änderungen
- 🛠️ Einfache Installation — eine einzige Variable

### 📦 Installation

```
1. Lege den Ordner max-speed in dein resources-Verzeichnis
2. Füge in server.cfg hinzu:
       ensure max-speed
3. Starte deinen Server neu
```

---

## 🇧🇷 Português

### 📖 Descrição

**max-speed** é um resource leve e universal para FiveM que impõe uma velocidade máxima a todos os veículos.  
Quando um veículo atinge o limite — fica **estável** nessa velocidade exata, sem piloto automático ou efeitos colaterais.

### ✅ Funcionalidades

- 🔒 Velocidade máxima configurável (padrão: **290 km/h**)
- ⚡ Extremamente leve — loop eficiente por frame
- 🎯 Aplica-se apenas ao motorista, não aos passageiros
- 🔄 Compatível com todos os frameworks sem modificação
- 🛠️ Instalação simples — uma única variável

### 📦 Instalação

```
1. Coloque a pasta max-speed no diretório resources
2. Adicione ao server.cfg:
       ensure max-speed
3. Reinicie o servidor
```

---

<div align="center">

## 📁 Estrutura dos Ficheiros / File Structure

```
max-speed/
├── fxmanifest.lua    # Resource manifest
├── client.lua        # Client-side speed limiter
├── server.lua        # Server-side logging
└── README.md         # This file
```

---

## ⚡ Performance

| Métrique | Valeur |
|----------|--------|
| Resmon (idle) | `~0.00 ms` |
| Resmon (in vehicle) | `~0.01 ms` |
| Scripts client | 1 |
| Scripts serveur | 1 |

---

*Made with ❤️ for FiveM Community*

**MIT License** — Free to use, modify and share.

</div>
