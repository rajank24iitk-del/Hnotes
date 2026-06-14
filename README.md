# हिंदी नोट्स — iPad Hindi Editor

Apple Pencil से हिंदी में परीक्षा पत्र और होमवर्क बनाने का PWA (Progressive Web App).

---

## GitHub Pages पर Deploy करने के चरण

### Step 1 — GitHub Account बनाएं (अगर नहीं है)
https://github.com/signup पर जाएं और free account बनाएं।

### Step 2 — नया Repository बनाएं
1. https://github.com/new खोलें
2. Repository name: `hindi-notes` (या कोई भी नाम)
3. **Public** चुनें (GitHub Pages के लिए जरूरी)
4. "Create repository" दबाएं

### Step 3 — Files Upload करें
1. नई repository में "uploading an existing file" link दबाएं
2. इन चारों files को drag-and-drop करें:
   - `index.html`
   - `manifest.json`
   - `sw.js`
   - `icon.svg`
3. "Commit changes" दबाएं

### Step 4 — GitHub Pages Enable करें
1. Repository में **Settings** tab खोलें
2. Left sidebar में **Pages** दबाएं
3. Source: **Deploy from a branch**
4. Branch: **main** → folder: **/ (root)**
5. **Save** दबाएं
6. 1-2 मिनट बाद आपका URL मिलेगा:
   `https://YOURNAME.github.io/hindi-notes/`

### Step 5 — iPad के Home Screen पर Install करें
1. iPad में **Safari** खोलें (Chrome नहीं — PWA के लिए Safari जरूरी है)
2. अपना GitHub Pages URL खोलें
3. नीचे **Share बटन** (□↑) दबाएं
4. **"Add to Home Screen"** चुनें
5. नाम: **हिंदी नोट्स** → **Add** दबाएं

अब app Home Screen पर icon की तरह दिखेगा और full-screen खुलेगा!

---

## App की विशेषताएं

| सुविधा | विवरण |
|--------|-------|
| ✏️ Apple Pencil | Pencil, Pen, Marker, Eraser — pressure sensitive |
| 🌿 Palm Rejection | हाथ रखने पर drawing नहीं होती |
| 📄 पृष्ठ सेटिंग | सादा, लाइन, ग्राफ — line spacing 0.5px accuracy तक |
| 💾 Presets | पसंदीदा page settings सहेजें और फिर load करें |
| 🎤 आवाज़ | हिंदी में बोलें, text canvas पर आ जाएगा |
| T  Scribble | Text mode में Apple Pencil से Scribble करें |
| 📑 PDF खोलें | पुराना PDF खोलें और उस पर लिखें |
| 📤 PDF सहेजें | हिंदी बिल्कुल सही — image के रूप में PDF में |
| ↩️ Undo/Redo | 60 steps तक |
| 🌈 24 रंग | + custom color picker + opacity |
| 📲 Offline | एक बार load होने के बाद internet बिना भी चलता है |

---

## हिंदी PDF की समस्या का समाधान

**पुरानी समस्या:** Word/PDF में हिंदी "जिबरिश" हो जाती थी।

**इस app का समाधान:** लिखाई को **image** के रूप में PDF में सहेजा जाता है।  
इससे हिंदी हमेशा बिल्कुल वैसी दिखती है जैसी लिखी गई थी।

---

## Shortcuts (Desktop पर test करते समय)

| Key | काम |
|-----|-----|
| `p` | Pen tool |
| `c` | Pencil tool |
| `m` | Marker tool |
| `e` | Eraser |
| `t` | Text mode |
| `Cmd+Z` | Undo |
| `Cmd+Shift+Z` | Redo |
| `Cmd+S` | Project सहेजें |
| `Cmd+P` | PDF export |

---

## File Format

Save करने पर `.hnotes` file बनती है (JSON format).  
इसे बाद में "प्रोजेक्ट खोलें" से load किया जा सकता है।

---

*Made with ❤️ for teachers*
