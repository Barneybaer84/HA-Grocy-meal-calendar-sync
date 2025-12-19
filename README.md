# Grocy Meal Plan to Calendar Sync for Home Assistant

This blueprint automates the synchronization of your **Grocy** meal plan with a Home Assistant calendar. It runs daily and ensures your dining schedule is always visible in your dashboard or calendar app.

[![Open your Home Assistant instance and show the blueprint import dialog with a specific blueprint pre-filled.](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https://raw.githubusercontent.com/Barneybaer84/HA-Grocy-meal-calendar-sync/refs/heads/main/grocy-meal-calendar_sync.yaml)

---

## 🌍 Languages / Sprachen
* **English** (Primary)
* **Deutsch** (German)

---

## 🚀 Features / Funktionen

### English
* **Smart Sync:** Only adds meals if they don't already exist on that specific day (Duplicate Check).
* **Customizable Prefix:** Add a custom text like "Meal: " or "Dinner: " before the recipe name.
* **Flexible Timing:** Choose exactly when the sync should happen every night.
* **Stability:** Optimized to avoid parser errors and handle missing data gracefully.

### Deutsch
* **Intelligenter Sync:** Fügt Mahlzeiten nur hinzu, wenn für diesen spezifischen Tag noch kein Eintrag mit demselben Namen existiert (Duplikatsprüfung).
* **Anpassbares Präfix:** Erlaube einen eigenen Text vor dem Rezeptnamen, z. B. „Essen: “ oder „Abendessen: “.
* **Flexible Zeitplanung:** Wähle selbst, zu welcher Uhrzeit die Synchronisierung jede Nacht stattfinden soll.
* **Stabilität:** Optimierter Code, um Parser-Fehler zu vermeiden und auch bei fehlenden Daten stabil zu laufen.

---

## 📋 Requirements / Voraussetzungen

### English
1. **Grocy Integration:** A working Grocy setup and the `sensor.grocy_meal_plan` entity.
2. **Writable Calendar:** You **MUST** use a calendar that allows creating events. 
   * ✅ **Supported:** Google Calendar, CalDAV, or the **Local Calendar integration** (created via *Settings -> Devices & Services -> Add Integration -> Local Calendar*).
   * ❌ **Not Supported:** Read-only calendars (like automatic holiday calendars or ICS-file imports).

### Deutsch
1. **Grocy Integration:** Eine funktionierende Grocy-Installation und die Entität `sensor.grocy_meal_plan`.
2. **Beschreibbarer Kalender:** Du **MUSST** einen Kalender verwenden, der das Erstellen von Ereignissen erlaubt.
   * ✅ **Unterstützt:** Google Calendar, CalDAV oder die **Lokale Kalender Integration** (erstellt unter *Einstellungen -> Geräte & Dienste -> Integration hinzufügen -> Lokaler Kalender*).
   * ❌ **Nicht unterstützt:** Schreibgeschützte Kalender (wie automatische Feiertagskalender oder ICS-Datei-Importe).

---

## ⚠️ Limitations / Einschränkungen

### English
Due to Home Assistant core limitations, automations currently cannot delete or move calendar events. 
* If you **reschedule or delete** a meal in Grocy, the old entry will remain in your calendar. 
* You will need to remove the outdated entry manually in the Calendar UI.

### Deutsch
Aufgrund von Einschränkungen im Home Assistant Core können Automatisierungen derzeit keine Kalenderereignisse löschen oder verschieben.
* Wenn du eine Mahlzeit in Grocy **verschiebst oder löschst**, bleibt der alte Eintrag im Kalender bestehen.
* Du musst den veralteten Eintrag manuell in der Kalender-Benutzeroberfläche entfernen.

---

## 🛠 Installation / Einrichtung

### English
1. Upload the `grocy_meal_plan_sync.yaml` to your `/blueprints/automation/` folder or use the **Import Button** above.
2. Go to **Settings -> Automations & Scenes -> Blueprints**.
3. Create a new automation from this blueprint.
4. Select your `sensor.grocy_meal_plan` and your target calendar.

### Deutsch
1. Lade die Datei `grocy_meal_plan_sync.yaml` in deinen Ordner `/blueprints/automation/` hoch oder nutze den **Import-Button** oben.
2. Gehe zu **Einstellungen -> Automatisierungen & Szenen -> Blueprints**.
3. Erstelle eine neue Automatisierung aus diesem Blueprint.
4. Wähle deinen `sensor.grocy_meal_plan` und deinen Ziel-Kalender aus.

---

## 📄 License
This blueprint is provided "as is". Feel free to modify and share it!
