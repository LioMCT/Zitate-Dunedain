# Stammeszitate – Waldläufer Dune Dain

Eine Website für die unvergesslichen Zitate des Stamms Dune Dain Waldläufer (VCP Baden).

## Inhalt

- `index.html` – Die Zitate-Website (eine einzige HTML-Datei, keine Dependencies)
- `vcp-logo.svg` – VCP Logo

## Neues Zitat hinzufügen

Öffne `index.html` und füge im Bereich `<!-- Zitat-Grid -->` einen neuen Block ein:

```html
<!-- Wer auch immer -->
<div class="quote-card card-feuerrot" data-author="benedikt">
  <p class="quote-text">Das Zitat hier rein.</p>
  <div class="quote-author">
    Benedikt
    <span class="badge-benedikt">Zitatemeister</span>
  </div>
</div>
```

### Verfügbare Kartenfarben (`class="quote-card ..."`)

| Klasse            | Farbe        |
|-------------------|--------------|
| `card-wasserblau` | Hellblau     |
| `card-feuerrot`   | Rot          |
| `card-feuergelb`  | Gelb         |
| `card-erdbraun`   | Dunkelbraun  |
| `card-dunkelblau` | Dunkelblau   |

### `data-author` Werte für den Filter

- `benedikt` – Zitat von Benedikt (zeigt ⭐-Badge)
- `unknown` – Unbekannte Quelle

### Für bekannte Person (kein Badge)

```html
<div class="quote-card card-wasserblau" data-author="max">
  <p class="quote-text">Das Zitat hier rein.</p>
  <div class="quote-author">Max</div>
</div>
```

> Tipp: Wenn du einen neuen Filter-Button für eine Person willst, kannst du in der `filter-bar` einen Button hinzufügen:
> ```html
> <button class="filter-btn" data-filter="max">Max</button>
> ```

## GitHub Pages hosting

1. Repository erstellen (z. B. `waldlaeufer-zitate`)
2. Diese Dateien pushen
3. Unter **Settings → Pages → Source**: Branch `main`, Ordner `/ (root)` wählen
4. Fertig! Die Website ist unter `https://<dein-username>.github.io/waldlaeufer-zitate/` erreichbar

## Design

Basiert auf den offiziellen **VCP Gestaltungsrichtlinien**:
- Schrift: Roboto
- Farben: VCP Blau (#004287), Wasserblau (#00b0eb), Feuerrot (#e94653), Feuergelb (#fecf16), Erdbraun (#603609)
