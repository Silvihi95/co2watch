# 🌍 CO₂Watch

> Transparenz über globale Treibhausgasemissionen – Fallstudie IPWA01-01  
> IU Internationale Hochschule · Kurs: Programmierung von Webanwendungsoberflächen

---

## 📋 Über das Projekt

**CO₂Watch** ist eine öffentlich zugängliche Webanwendung, die fiktive CO₂-Emissionsdaten von Ländern und Unternehmen übersichtlich darstellt. Das Projekt wurde im Rahmen der Fallstudie IPWA01-01 (Aufgabe 1.1) an der IU Internationalen Hochschule entwickelt.

🔗 **Live-Demo:** [https://Silvihi95.github.io/co2watch/](https://Silvihi95.github.io/co2watch/)  
*(Link nach Aktivierung von GitHub Pages ersetzen)*

> ⚠️ Alle dargestellten Daten sind vollständig fiktiv und dienen ausschließlich zu Demonstrationszwecken.

---

## ✅ Umgesetzte Anforderungen

| # | Anforderung | Status |
|---|---|---|
| a | Titel und Logo | ✅ |
| b | Header mit globaler Navigation, Content-Bereich, Footer mit Rechtspflichten | ✅ |
| c | Menü mit lokalen Links – LTR/RTL-Umschaltung je nach Schriftkultur | ✅ |
| d | Responsives Design (Desktop, Tablet, Smartphone) | ✅ |
| e | Sortier- und filterbare CO₂-Emissionstabelle (Land, Unternehmen, Sektor) | ✅ |
| f | Absicherung aller Eingabefelder gegen Code-Injection (XSS-Schutz) | ✅ |

---

## 🛠️ Technologien

- **HTML5** – Semantische Struktur, ARIA-Accessibility
- **CSS3** – Custom Properties, CSS Grid, Flexbox, Media Queries
- **Vanilla JavaScript** – Keine externen Frameworks, keine Build-Tools
- **Google Fonts** – Syne (Display) + Space Mono (Mono)

---

## 📁 Projektstruktur

```
co2watch/
├── index.html        # Vollständige Single-Page-Anwendung
└── README.md         # Diese Datei
```

---

## 🔒 Sicherheit

Alle Eingabefelder sind gegen Cross-Site-Scripting (XSS) abgesichert:

- **`sanitize()`** – Bereinigt Eingaben in Echtzeit (`oninput`-Event), entfernt HTML-Tags, Event-Handler-Muster und gefährliche Schlüsselwörter
- **`escapeHTML()`** – Maskiert alle Sonderzeichen vor der DOM-Insertion (`&`, `<`, `>`, `"`, `'`, `/`)
- **`maxlength`-Attribute** – Begrenzen die Eingabelänge auf Formularebene

---

## 📱 Responsive Breakpoints

| Breakpoint | Verhalten |
|---|---|
| > 900px | Zweispaltiges Layout mit Sidebar-Navigation |
| ≤ 900px | Einspaltig, Sidebar ausgeblendet |
| ≤ 640px | Hamburger-Menü, 2-spaltige Statistik-Karten |

---

## ⚖️ Rechtliches

Die Webseite enthält vollständige rechtliche Seiten (aufrufbar über Footer-Links):

- Impressum (§ 5 TMG)
- Datenschutzerklärung (DSGVO)
- Nutzungsbedingungen
- Barrierefreiheitserklärung (WCAG 2.1 AA)
- Quellenangaben
- Methodik

---

## 👤 Autor

Silvia H.
Matrikelnummer: 3211*****
IU Internationale Hochschule  
Kurs: IPWA01-01 – Programmierung von Webanwendungsoberflächen

---

## 📄 Lizenz

Dieses Projekt wurde im Rahmen einer Prüfungsleistung erstellt.  
© [Silvia H.] · IU Internationale Hochschule · 2026
