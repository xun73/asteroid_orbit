# 小行星軌道與天球互動模擬器 | Asteroid Orbit & Celestial Sphere Simulator

[繁體中文](#繁體中文) · [English](#english)

線上使用 | Live demo: [https://xun73.github.io/asteroid_orbit/](https://xun73.github.io/asteroid_orbit/)

## 繁體中文

這是一個以 Three.js 製作的互動式天文模擬器，可在太陽系日心視圖中觀察軌道，也能查看從地球方向投影到天球上的位置。程式以單一 HTML 頁面執行，不需要後端或代理服務。

### 功能

- **同步視圖：**以 3D 日心視圖和地心天球視圖觀察小行星與地球。
- **軌道參數：**調整半長軸 `a`、離心率 `e`、傾角 `i`、升交點黃經 `Ω`、近日點幅角 `ω`、平近點角 `M` 與曆元。
- **快速載入：**載入金星、木星、冥王星、穀神星、法厄同、阿波菲斯、貝努、哈雷彗星或恩克彗星的範例軌道。
- **行星參考軌道：**可切換顯示水星至海王星的軌道，方便比較小行星軌道位置。
- **時間控制：**播放、暫停、反向播放或調整模擬日期與速度。
- **MPC 軌道資料：**將 MPCORB 的小行星固定欄位資料貼入程式，解析後載入軌道參數。
- **MPC 觀測資料：**貼上 MPC 觀測記錄並標示觀測位置，也可設定日期範圍。
- **語言：**中文瀏覽器自動使用繁體中文；其他語言預設英文。可用右上角按鈕手動切換。

### 載入 MPC 資料

1. 在上方 MPC 搜尋欄輸入小行星名稱或編號，按放大鏡開啟 MPC 天體頁面。
2. 若要載入軌道，從 MPCORB 資料取得該天體的固定欄位記錄，貼入 **MPCORB Orbital Elements Parser**，按 **Parse & Load Orbit**。
3. 若要顯示觀測位置，從 MPC 資料頁複製觀測記錄，貼入 **MPC Observation Report Markers**，按 **Parse & Mark**；需要時設定起訖日期並套用區間。

MPC 天體搜尋會開啟 MPC 網站；軌道與觀測資料由使用者自行複製貼入，不會透過本程式自動下載。

### 執行方式

- **線上：**開啟上方 GitHub Pages 連結。
- **本機：**下載或複製此儲存庫後，以瀏覽器開啟 `index.html`。程式使用 Three.js、OrbitControls 和 Tailwind CSS 的 CDN，載入頁面時需要網路連線。

### 模型說明

軌道位置以克卜勒二體模型近似計算，適合互動觀察與教學用途；不等同於 MPC 或 JPL 的高精度星曆，也未模擬所有天體攝動。

### 技術

- HTML5、JavaScript (ES6+)
- [Three.js r128](https://threejs.org/)
- [Tailwind CSS](https://tailwindcss.com/)

## English

An interactive astronomy simulator built with Three.js. Explore orbits in a heliocentric Solar System view and inspect object directions projected onto a geocentric celestial sphere. The app runs as a single HTML page and requires no backend or proxy service.

### Features

- **Synchronized views:** Explore asteroid and Earth positions in 3D heliocentric and geocentric celestial-sphere views.
- **Orbital elements:** Adjust semi-major axis `a`, eccentricity `e`, inclination `i`, longitude of ascending node `Ω`, argument of perihelion `ω`, mean anomaly `M`, and epoch.
- **Quick Load:** Load example orbits for Venus, Jupiter, Pluto, Ceres, Phaethon, Apophis, Bennu, Halley's Comet, and Encke's Comet.
- **Planetary reference orbits:** Toggle the Mercury-through-Neptune orbits to compare asteroid orbit positions.
- **Time controls:** Play, pause, reverse, and adjust the simulated date and speed.
- **MPC orbital data:** Paste a numbered asteroid's MPCORB fixed-width record to parse and load its orbital elements.
- **MPC observations:** Paste MPC observation records to mark observation positions, with an optional date-range filter.
- **Languages:** Chinese browser locales select Traditional Chinese automatically; all other locales default to English. Use the button in the upper-right corner to switch manually.

### Loading MPC data

1. Enter an asteroid name or number in the MPC search field and click the magnifier to open its MPC object page.
2. To load an orbit, copy the object's fixed-width record from MPCORB, paste it into **MPCORB Orbital Elements Parser**, and click **Parse & Load Orbit**.
3. To show observation positions, copy observation records from an MPC data page, paste them into **MPC Observation Report Markers**, and click **Parse & Mark**. Set and apply a date range if needed.

MPC search opens the MPC website. Users copy and paste orbital or observation data themselves; the app does not download MPC data automatically.

### Running the app

- **Online:** Open the GitHub Pages link above.
- **Locally:** Download or clone this repository, then open `index.html` in a browser. The app loads Three.js, OrbitControls, and Tailwind CSS from CDNs, so an internet connection is required when loading the page.

### Model notes

Orbital positions use an approximate Keplerian two-body model for interactive exploration and education. They are not a substitute for high-precision MPC or JPL ephemerides and do not model all gravitational perturbations.

### Technology

- HTML5 and JavaScript (ES6+)
- [Three.js r128](https://threejs.org/)
- [Tailwind CSS](https://tailwindcss.com/)

---

Developed by [xun73](https://github.com/xun73)
