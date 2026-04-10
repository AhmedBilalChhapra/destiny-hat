# 🎩 Global Destiny Hat - Interactive Lead-Gen Tool

An interactive, high-conversion web application developed for **EdPro Consultants**. This tool uses a "Sorting Hat" gamification logic to match prospective students with their ideal study-abroad destination while capturing high-intent lead data.

## 🚀 Live Demo
**View the project in action:** [https://abcthe24th-dot.github.io/destiny-hat/](https://abcthe24th-dot.github.io/destiny-hat/)

## 🛠️ Key Features
* **Dynamic Sorting Logic:** A 7-question psychological assessment that calculates destination affinity across 8 global regions (UK, USA, Australia, Canada, Germany, UAE, Malaysia, and New Zealand).
* **Automated Lead Capture:** Integrated with Google Apps Script API to push student contact data (Name, Email, WhatsApp) directly to a centralized Google Sheet in real-time.
* **Social Share Engine:** Uses `html2canvas` with custom CORS handling to generate high-definition (2x scale) result cards ready for Instagram Stories.
* **Mobile-First Design:** Fully responsive UI built with modern CSS variables, optimized for high engagement on mobile browsers.

## 💻 Tech Stack
* **Frontend:** HTML5, CSS3, JavaScript (ES6+)
* **Libraries:** [html2canvas](https://html2canvas.hertzen.com/) for client-side image generation.
* **Backend Integration:** Google Apps Script / Google Sheets API.
* **Deployment:** GitHub Pages.

## 🔧 Technical Challenges & Solutions
### 🖼️ Cross-Origin Resource Sharing (CORS)
**Challenge:** Initially, the Instagram sharing feature failed due to "Tainted Canvas" errors when trying to capture local image assets in a live environment.
**Solution:** Implemented `crossorigin="anonymous"` on image elements and configured the `html2canvas` settings to allow cross-origin resource sharing, ensuring seamless image generation.

### 📱 High-Definition Capture
**Challenge:** Standard screenshots appeared blurry on high-end smartphone displays (Retina/OLED).
**Solution:** Programmed a custom scaling factor (`scale: 2`) within the capture logic to ensure result cards remain crisp when uploaded to social media.

## 📂 Project Structure
```text
├── index.html          # Core application logic and styling
├── images/             # Optimized destination assets
│   ├── us.jpg          # USA Landmark
│   ├── germany.jpg     # Germany Landmark
│   └── ...             # [Other 6 destinations]
└── README.md           # Project documentation

👤 Developer
Ahmed Bilal Chhapra
Brand Ambassador | EdPro Consultants
