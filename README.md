# 🧰 Getting Started with Scrooch 3

Welcome to the **Scrooch 3 Modding Framework**! This guide will help you set up and customize your own Scratch mod powered by Scrooch.

---

## 🧪 1. Duplicate the Template

To get started, click this link:

👉 [**Create Your Scrooch 3 Mod**](https://github.com/new?template_name=Scrooch3-Template&template_owner=scrooch-project&use_v2_form=false)

---

## 🌍 2. Enable GitHub Pages

After duplicating your repository:

1. Go to **Settings > Pages**
2. Under **Source**, select:

   * Branch: `main`
   * Folder: `/ (root)`
3. GitHub will give you a public link like:

   ```
   https://your-username.github.io/your-mod-name
   ```

If it doesn't work right away, try turning Pages off and on again, or wait a few minutes.

---

## 🖼️ 3. Replace Icons & Assets

You can change the look of your editor by replacing SVGs. For example:

| File Path                                            | Description                                                             |
| ---------------------------------------------------- | ----------------------------------------------------------------------- |
| `static/assets/10db5ce4c37ebd51abc46eb6840d4cfa.svg` | Stop button icon                                                        |
| `static/assets/9525874be2b1d66bd448bf53400011a9.svg` | Green Flag icon (main UI)                                               |
| `static/blocks-media/green-flag.svg`                 | "When Flag Clicked" block icon                                          |
| `static/blocks-media/blue-flag.svg`                  | Alternate "When Flag Clicked" icon (used for themes or visual variants) |

---

## 📝 4. Change the Page Titles

In **both** `editor.js` and `js/player.js`, use `Ctrl+F` to find:

```
PenguinMod -
```

Then:

* Replace `"PenguinMod"` with the name you want in the browser title.
* Look 2 lines below and change `"PenguinMod"` again to your mod's name.

---

## 🔗 5. Edit Footer Links

You can replace the default footer links (like "TurboWarp Packager", "Embedding", "Source Code") with your own.

### ✅ To do this:

1. Open **`editor.js`** and **`js/player.js`**
2. Use `Ctrl+F` and search for:

```
TurboWarp Packager
```

3. You’ll find link blocks like this:

```js
}, 'TurboWarp Packager'), /*#__PURE__*/react__WEBPACK_IMPORTED_MODULE_2___default.a.createElement("a", {
  href: "https://docs.turbowarp.org/embedding"
}, 'Embedding'), /*#__PURE__*/react__WEBPACK_IMPORTED_MODULE_2___default.a.createElement("a", {
  href: "https://docs.turbowarp.org/url-parameters"
}, 'URL Parameters'), /*#__PURE__*/react__WEBPACK_IMPORTED_MODULE_2___default.a.createElement("a", {
  href: "https://github.com/TurboWarp/packager"
}, 'Source Code'),
```

4. Edit the `'text'` and the `"href"` to point to your own docs or site.

❗️ Do **not** delete entire JSX blocks — just update the content and URLs.
