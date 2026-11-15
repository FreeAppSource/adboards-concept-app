# Adboards Concept App

> 👨‍💻 Developed by **[Suresh Kumar Meesala](https://github.com/SureshKumarMeesala)** · 🎨 UI design by **Ahmad Firoz** (credits below)

A mobile app built with **React Native (0.88+)**, **Expo SDK 58+** and **Expo Router**, using **JavaScript and JSX (`.js`, `.jsx`)**. Every screen is built from the original Sketch design `adborads-app-concept-ahmadfiroz.sketch` by **Ahmad Firoz**: one route per artboard, with the artboard's layout, colours, images and text.

![Adboards Concept App screens](./showcase.jpg)

## 📱 Screens (11 design artboards)

Listed in the order of the app's flow. "Taps" is the number of tap targets wired on the screen (buttons, tabs, back arrows, list rows).

| # | Screen (artboard) | Route | Size | Taps |
|---|---|---|---|---|
| 1 | **Login** · start screen | `src/app/login.jsx` | 375 × 812 | 3 |
| 2 | **Expertise level** | `src/app/expertise-level.jsx` | 375 × 812 | 5 |
| 3 | **Campaigns -- Normal** | `src/app/campaigns-normal.jsx` | 375 × 812 | 3 |
| 4 | **Campaigns -- None** | `src/app/campaigns-none.jsx` | 375 × 812 | 2 |
| 5 | **Campaigns -- Category** | `src/app/campaigns-category.jsx` | 375 × 812 | 4 |
| 6 | **Tamplate -- Details** | `src/app/tamplate-details.jsx` | 375 × 939 | 4 |
| 7 | **Campaigns -- Form** | `src/app/campaigns-form.jsx` | 375 × 812 | 4 |
| 8 | **Tamplate -- Editor** | `src/app/tamplate-editor.jsx` | 375 × 812 | 4 |
| 9 | **Tamplate -- Choose** | `src/app/tamplate-choose.jsx` | 375 × 963 | 7 |
| 10 | **Tamplate -- Select** | `src/app/tamplate-select.jsx` | 375 × 873 | 4 |
| 11 | **Campaigns -- Done** | `src/app/campaigns-done.jsx` | 375 × 812 | 5 |

Screenshots of every screen are in [`screenshots/`](./screenshots).

## 🧩 How it's built

- `src/screens/*.json`: each design artboard converted to screen data (vector shapes, gradients, image fills, masks, shadows, blurs and rich text, positioned as in the design), plus its tap targets
- `src/sketch/SketchScreen.jsx`: draws a screen at the device's width with `react-native-svg`, native `Text`/`TextInput` and `expo-blur`, and handles navigation between screens
- `src/app/`: Expo Router routes, one per artboard (`index.jsx` opens the start screen)
- `assets/images/`: images used by the design

## 🛠️ Tech Stack

- **Framework**: React Native 0.88+ / Expo SDK 58+
- **Navigation**: Expo Router (file-based routing)
- **Language**: JavaScript & JSX (`.js`, `.jsx`)
- **Rendering**: `react-native-svg`, `expo-blur`
- **Fonts**: Google Fonts via `@expo-google-fonts` (Inter), standing in for the design's original fonts where those aren't free

<!-- run-locally:start -->

## ▶️ Run locally

```bash
npm install
npx expo start
```

Then press `i` for the iOS simulator, `a` for Android, or `w` for the web, or scan the QR code with Expo Go.

<!-- run-locally:end -->

<!-- developer:start -->

## 👨‍💻 Developer

This React Native app was developed by **Suresh Kumar Meesala**.

| | |
|---|---|
| Developer | [Suresh Kumar Meesala](https://github.com/SureshKumarMeesala) |
| GitHub | [@SureshKumarMeesala](https://github.com/SureshKumarMeesala) |
| Organization | [FreeAppSource](https://github.com/FreeAppSource) |
| Repository | <https://github.com/FreeAppSource/adboards-concept-app> |

<!-- developer:end -->

---

<!-- design-credits:start -->

## 🎨 Design Credits

This app is based on the free **Adboards AR App Concept** design by **Ahmad Firoz**, downloaded from Sketch App Sources. All visual design credit goes to the designer. The screens are reproduced from the original Sketch file; fonts that aren't free are replaced with similar Google Fonts, so some details may differ slightly from the original.

| | |
|---|---|
| Designer | [Ahmad Firoz](https://www.sketchappsources.com/contributor/ahmadfiroz) |
| Original design | [Adboards AR App Concept](https://dribbble.com/shots/10724951-Adboards-Free-Sketch-File) |
| Downloaded from | [Sketch App Sources](https://www.sketchappsources.com/free-source/4365-adborads-app-concept-sketch-freebie-resource.html) |
| Dribbble | <http://www.dribbble.com/ahmadfiroz> |
| Twitter | <https://twitter.com/firoz_usf> |
| Website | <http://ahmadfiroz.com/> |
| Original file | `adborads-app-concept-ahmadfiroz.sketch` |
| License / usage | Not stated on the page. Free download; give credit (Sketch App Sources Terms). Confirm with the designer before commercial use. |

**Attribution:**

> UI design: "Adboards AR App Concept" by Ahmad Firoz (https://dribbble.com/shots/10724951-Adboards-Free-Sketch-File), downloaded from Sketch App Sources (https://www.sketchappsources.com/free-source/4365-adborads-app-concept-sketch-freebie-resource.html).

The original design source files are not included in this repository; get them from the links above. This app's **code** is released under the [MIT License](./LICENSE); the visual design remains the designer's (see [NOTICE](./NOTICE)).

Photos, brand logos and avatars inside the design may belong to third parties and are not covered by the designer's permission.

<!-- design-credits:end -->
