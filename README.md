# Grocy Meal Plan to Calendar Sync / Speiseplan Kalender-Sync

[![Open your Home Assistant instance and show the blueprint import dialog with a specific blueprint pre-filled.](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https://raw.githubusercontent.com/Barneybaer84/HA-Grocy-meal-calendar-sync/refs/heads/main/grocy-meal-calendar_sync.yaml)

### 🌍 Languages / Sprachen
* **English** (Primary)
* **Deutsch** (German)

---

## 🇺🇸 English Description

This Blueprint automatically synchronizes your planned meals from **Grocy** to a **Home Assistant Calendar**. It ensures that you have your meal plan and cooking instructions everywhere you go.

### ✨ Key Features
* **Full Sync:** Automatically synchronizes your meal plan for the next 7 days.
* **Recipe Instructions:** Includes preparation steps directly in the calendar event description.
* **Smart Formatting:** Uses specialized logic to convert Grocy's HTML instructions into clean text lists with forced line breaks for maximum compatibility with external apps (Google, Apple, etc.).
* **Duplicate Prevention:** Checks each day for existing events to avoid cluttered calendars.

### 🛠 Requirements
* **Grocy Integration:** A working Grocy integration with an active `sensor.grocy_meal_plan`.
* **Calendar:** A writable calendar in Home Assistant (e.g., **Local Calendar** helper or **Google Calendar** integration).
* **Recipe Descriptions:** Ensure your Grocy recipes have text in the "Description" field to see instructions in your calendar.

### 🚀 Installation
1. Click the "Import" button above or go to **Settings > Automations > Blueprints** in Home Assistant.
2. Click **Import Blueprint** and paste this URL:
   `https://github.com/Barneybaer84/HA-Grocy-meal-calendar-sync/blob/main/grocy-meal-calendar_sync.yaml`

---

## 🇩🇪 Deutsche Beschreibung

Dieser Blueprint synchronisiert deinen geplanten Speiseplan von **Grocy** automatisch mit einem **Home Assistant Kalender**. So hast du deinen Plan und die Kochanleitungen immer griffbereit.

### ✨ Hauptfunktionen
* **Vollständiger Sync:** Synchronisiert automatisch den Speiseplan der nächsten 7 Tage.
* **Zubereitungsanleitung:** Fügt die Kochschritte direkt in die Beschreibung des Kalendertermins ein.
* **Intelligente Formatierung:** Nutzt eine spezielle Logik, um HTML-Anleitungen aus Grocy in saubere Textlisten mit erzwungenen Zeilenumbrüchen umzuwandeln (optimiert für Google Kalender, Apple Kalender etc.).
* **Duplikatschutz:** Prüft jeden Tag auf vorhandene Einträge, um Dopplungen zu vermeiden.

### 🛠 Voraussetzungen
* **Grocy Integration:** Eine funktionierende Grocy-Integration mit einem aktiven `sensor.grocy_meal_plan`.
* **Kalender:** Ein beschreibbarer Kalender in Home Assistant (z. B. der **Lokaler Kalender** Helfer oder die **Google Kalender** Integration).
* **Rezept-Beschreibungen:** Damit Anleitungen im Kalender erscheinen, müssen deine Grocy-Rezepte Text im Feld "Beschreibung" enthalten.

### 🚀 Installation
1. Klicke auf den "Import"-Button oben oder gehe in Home Assistant zu **Einstellungen > Automatisierungen & Szenen > Blueprints**.
2. Klicke auf **Blueprint importieren** und füge diese URL ein:
   `https://github.com/Barneybaer84/HA-Grocy-meal-calendar-sync/blob/main/grocy-meal-calendar_sync.yaml`

---

## 💡 Technical Notes / Technische Hinweise

### 🇺🇸 English
* **Line Breaks:** Due to Home Assistant UI limitations, line breaks might look more compact in the internal HA calendar, but will appear as a perfect vertical list in external apps like Google Calendar.
* **No Auto-Deletion:** Home Assistant currently does not support deleting calendar events via automation. If you move or delete a meal in Grocy, the existing calendar entry must be removed manually.

### 🇩🇪 Deutsch
* **Zeilenumbrüche:** Aufgrund von Einschränkungen der HA-Benutzeroberfläche erscheinen Zeilenumbrüche im internen Kalender kompakter, werden aber in externen Apps wie Google Kalender als saubere Liste untereinander angezeigt.
* **Keine automatische Löschung:** Home Assistant unterstützt aktuell keine Löschung von Kalendereinträgen per Automatisierung. Wenn du eine Mahlzeit in Grocy verschiebst oder löschst, muss der vorhandene Kalendereintrag manuell entfernt werden.

---
*Created by [Barneybaer84](https://github.com/Barneybaer84)*
