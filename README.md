# 🌾 SaruKetha (සරු කෙත) — Direct Farm-to-Buyer Marketplace | ගොවියාගෙන් කෙලින්ම වෙළෙන්දාට

**SaruKetha** is a direct-to-buyer agricultural marketplace web application designed to eliminate exploitative middlemen in Sri Lanka's agricultural supply chain. By connecting local farmers directly with wholesale and retail buyers, SaruKetha ensures fair farm-gate pricing for growers and fresher produce at transparent rates for sellers.

**සරු කෙත (SaruKetha)** යනු ශ්‍රී ලංකාවේ කෘෂිකාර්මික සැපයුම් දාමය තුළ සිටින අතරමැදියන්ගේ බලපෑම අවම කරමින්, ගොවියා සහ වෙළෙන්දා සෘජුවම සම්බන්ධ කිරීම සඳහා නිර්මාණය කරන ලද වෙබ් යෙදුමකි. මෙමගින් ගොවීන්ට තම අස්වැන්න සඳහා සාධාරණ මිලක් ලබා ගැනීමටත්, වෙළෙන්දන්ට අතරමැදි ගාස්තු වලින් තොරව නැවුම් නිෂ්පාදන සෘජුවම මිලදී ගැනීමටත් අවස්ථාව සැලසේ.

---

## 📖 Problem Statement & Solution | ගැටලුව සහ විසඳුම

### The Problem (ගැටලුව)
In Sri Lanka, smallholder farmers often receive disproportionately low prices for their harvests due to multiple layers of intermediaries and brokers between the farm gate and economic centers (such as Dambulla, Keppetipola, and Pettah). Meanwhile, retail sellers and consumers still pay inflated prices for produce that has lost freshness in transit.

ශ්‍රී ලංකාවේ ගොවීන් සහ ආර්ථික මධ්‍යස්ථාන (දඹුල්ල, කැප්පෙටිපොළ, පිටකොටුව වැනි) අතර විශාල අතරමැදියන් සහ තැරැව්කරුවන් පිරිසක් සිටීම නිසා ගොවීන්ට තම අස්වැන්නට සාධාරණ මිලක් නොලැබේ. එමෙන්ම ප්‍රවාහනයේදී නැවුම් බව අඩු වූ එළවළු සහ පලතුරු සඳහා වෙළෙන්දන්ට සහ පාරිභෝගිකයන්ට ඉහළ මිලක් ගෙවීමට සිදු වේ.

### The Solution (විසඳුම)
**SaruKetha** provides a streamlined digital platform where:
* **Farmers** can list their available harvest stock directly, set their own fair price per kilogram, and manage incoming buyer orders.
* **Buyers / Sellers** can browse real-time crop availability across districts, compare prices against standard economic center rates, and purchase directly from farmers without middleman markups.

**සරු කෙත** හරහා පහත පහසුකම් සැලසේ:
* **ගොවීන්ට (Farmers):** තමන් සතු අස්වැන්න පිළිබඳ විස්තර, කිලෝග්‍රෑම් එකක සාධාරණ මිල සහ ප්‍රමාණය පද්ධතියට ඇතුළත් කිරීමටත්, ලැබෙන ඇණවුම් කළමනාකරණය කිරීමටත් හැකියාව ලැබේ.
* **වෙළෙන්දන්ට (Buyers / Sellers):** දිවයිනේ විවිධ දිස්ත්‍රික්කවල ගොවීන් සතු අස්වැන්න පරීක්ෂා කර, ආර්ථික මධ්‍යස්ථාන මිල ගණන් සමඟ සසඳා අතරමැදියන්ගෙන් තොරව ගොවියාගෙන්ම සෘජුව මිලදී ගත හැකිය.

---

## ✨ Key Features | ප්‍රධාන විශේෂාංග

* **Dual-Role Experience (ද්විත්ව පරිශීලක අත්දැකීම):** Seamless switching between **Farmer Portal** (ගොවි පුවරුව) and **Buyer Marketplace** (වෙළඳපොළ) views.
* **Farmer Stock Management (අස්වැන්න කළමනාකරණය):** Add new harvest listings (crop type, district, available weight in kg, price in LKR, harvest date), edit existing stock, and manage availability.
* **Direct Order Fulfillment (සෘජු ඇණවුම් කළමනාකරණය):** Farmers receive incoming purchase requests and can accept or decline orders, automatically updating remaining stock levels.
* **Smart Marketplace Filtering (පහසු සෙවුම් පහසුකම්):** Buyers can search by crop name and filter listings by category, district, and maximum price per kg.
* **Wholesale Price Reference (තොග මිල සැසඳීම):** Built-in comparison against average economic center wholesale rates to highlight direct-purchase savings.
* **Client-Side Persistence (දත්ත ගබඩා කිරීම):** Powered by browser `localStorage` with pre-seeded Sri Lankan agricultural data for immediate demonstration.

---

## 🛠️ Tech Stack & Constraints | තාක්ෂණය සහ සීමාවන්

* **Frontend:** Semantic HTML5, Modern CSS3 (Flexbox, Grid, CSS Variables), Vanilla JavaScript (ES6+)
* **Data Persistence:** Browser `localStorage` (JSON-based state management)
* **Development Standard:** Built 100% from scratch without external frameworks, libraries, or AI-generated code. (කිසිදු බාහිර framework එකක් හෝ AI මෙවලමක් භාවිතා නොකර 100% ක්ම අප විසින්ම නිර්මාණය කරන ලදී.)

---

## 📂 Project Structure | ව්‍යාපෘති ව්‍යුහය

```text
saruketha/
├── index.html              # Landing page & Wholesale Price Ticker
├── login.html              # Role Switcher / Mock Authentication
├── marketplace.html        # Buyer view: Browse, filter & order crops
├── dashboard.html          # Farmer view: Stock & order management
├── css/
│   ├── global.css          # Design tokens, typography, navbar & layout
│   ├── marketplace.css     # Product grid, filter controls & order modal
│   └── dashboard.css       # Forms, analytics cards & order tables
├── js/
│   ├── data.js             # Pre-loaded Sri Lankan farmer & crop seed data
│   ├── storage.js          # localStorage CRUD helper utilities
│   ├── auth.js             # Active user session & role management
│   ├── marketplace.js      # Dynamic rendering, filtering & order logic
│   └── dashboard.js        # Stock creation, updates & order approval
└── assets/
    └── images/             # Crop thumbnails & UI icons
```

---

## 🚀 Getting Started | ආරම්භ කරන ආකාරය

1. **Clone the repository (ව්‍යාපෘතිය බාගත කරන්න):**
   ```bash
   git clone https://github.com/your-username/saruketha.git
   ```
2. **Navigate to the project directory (ෆෝල්ඩරය වෙත පිවිසෙන්න):**
   ```bash
   cd saruketha
   ```
3. **Run the application (යෙදුම ක්‍රියාත්මක කරන්න):**
   * Open `index.html` directly in any modern web browser, **or**
   * Use the **Live Server** extension in VS Code for hot-reloading during development.

---

## 👥 Co-Developers | සම-සංවර්ධකයින්

This project was collaboratively designed and developed by (මෙම ව්‍යාපෘතිය සාමූහිකව නිර්මාණය කර සංවර්ධනය කරන ලද්දේ):

1. **[Member 1 Name]** — *UI/UX Design & Responsive CSS Architecture* ([@github-handle-1](https://github.com/))
2. **[Member 2 Name]** — *Farmer Dashboard & Inventory Logic* ([@github-handle-2](https://github.com/))
3. **[Member 3 Name]** — *Buyer Marketplace, Search & Filtering* ([@github-handle-3](https://github.com/))
4. **[Member 4 Name]** — *State Management (`localStorage`) & Order Workflow* ([@github-handle-4](https://github.com/))
5. **[Member 5 Name]** — *Role Authentication, Seed Data & QA Testing* ([@github-handle-5](https://github.com/))

---

*Developed as part of the Web Development Module Group Project. | වෙබ් සංවර්ධන මොඩියුලයේ කණ්ඩායම් ව්‍යාපෘතියක් ලෙස නිර්මාණය කරන ලදී.*
