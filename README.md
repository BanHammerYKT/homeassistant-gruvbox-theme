# 🎨 Home Assistant Gruvbox Theme

A warm, retro-inspired theme for Home Assistant, based on the earthy colours and soft contrast of [gruvbox](https://github.com/morhetz/gruvbox).

Gruvbox is designed to feel comfortable over long sessions: muted backgrounds, readable text, and accents that stand out without turning the whole dashboard neon. This theme brings that same calm, slightly nostalgic feeling to Home Assistant, with matching light and dark modes and a few extra touches for popular Lovelace cards.

## 📸 Screenshots

### Light

![Light theme screenshot](https://raw.githubusercontent.com/kizza/homeassistant-gruvbox-theme/main/assets/screenshots/light.png)

### Dark

![Dark theme screenshot](https://raw.githubusercontent.com/kizza/homeassistant-gruvbox-theme/main/assets/screenshots/dark.png)

## 📦 Installation

### HACS

Install with [HACS](https://hacs.xyz/) for the easiest setup and future updates:

1. Open HACS in Home Assistant.
2. Go to **Frontend**.
3. Search for **Gruvbox Theme**.
4. Install the theme, then restart Home Assistant.
5. Select **Gruvbox** from your profile theme settings.

If it does not appear in search yet, add `https://github.com/kizza/homeassistant-gruvbox-theme` as a custom HACS theme repository first.

### Manual

Clone this repository and place `themes/gruvbox.yaml` into your Home Assistant `themes/` folder.

Add the following code to your `configuration.yaml` file (reboot required).

```yaml
frontend:
  ... # your configuration.
  themes: !include_dir_merge_named themes
  ... # your configuration.
```

## ✨ Features

- Light and dark modes, with Home Assistant's automatic mode switching supported.
- Warm, low-contrast surfaces inspired by the original editor theme.
- Gruvbox accent colours mapped across Home Assistant UI variables.
- Extra colour variables for [Mushroom](https://github.com/piitaya/lovelace-mushroom) cards.
- Works as a normal Home Assistant frontend theme, so each user can choose it from their own profile settings.

## 💡 Notes

- After installing or updating the theme, restart Home Assistant if the new colours do not appear immediately.
- If your browser keeps showing an older version, clear the frontend cache or reload Home Assistant with cache disabled.

## 🛠 Development

The theme YAML is generated from TypeScript source files. To rebuild it locally, run:

```bash
bun install
bun run build
```
