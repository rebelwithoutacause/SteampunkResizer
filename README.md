# Steampunk Lever Size Converter — EU → US

A vintage-steampunk-style web app that converts European (EU) clothing sizes to their approximate US equivalents. Users pull a mechanical lever to execute the conversion — just like an old machine!

![Steampunk Lever UI](SteampunkResizer/SteampunkResizer/Screenshot.png)



  
*Example of the app interface with lever and gears.*

---

## Features

- **Steampunk Style UI**: Panels, gears, levers, and brass textures for a mechanical feel.
- **Lever-based Interaction**: Pull the lever or click/press a button to perform the conversion.
- **Category Support**:  
  - Women — dresses/tops  
  - Men — pants (waist) and jackets (chest)  
  - Children — size approximated from height (cm)
- **Keyboard Accessible**: Navigate fields and operate lever using Enter or Space keys.
- **Web and Desktop Ready**:  
  - Open in any modern browser.  
  - Can be wrapped in Electron or Tauri for downloadable desktop apps.

---

## Conversion Logic

- **Women**: Uses a lookup table for standard EU sizes; interpolates for in-between values.  
- **Men Pants**: US waist = EU size − 16  
- **Men Jackets**: US chest = EU size − 10  
- **Children**: EU size matched to approximate age/height categories  

> ⚠️ Conversions are approximate and intended as guidelines.

---

## Usage

1. Open `index.html` in a browser.
2. Select a **category**.
3. Enter the **EU size**.
4. Pull the lever, click the button, or press **Enter** to see the US size result.

---

## Installation / Desktop App

To create a downloadable app, you can wrap this project using:

- **Electron** (JavaScript desktop apps)
- **Tauri** (lightweight Rust-based wrapper)
- **Flutter** (multi-platform: web, desktop, mobile)

Check the inline comments in `index.html` for step-by-step packaging instructions.

---

## Accessibility

- ARIA attributes for screen readers.
- Keyboard navigation (tab to lever or input fields, use Enter/Space to convert).
- Motion-reduced mode compatible (lever animation can be disabled if needed).

---

## Contributing

Contributions, ideas, and bug reports are welcome!  
Feel free to open an issue or submit a pull request.

---

## License

This project is open-source under the MIT License.
