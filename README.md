# Asteroid Orbit & Celestial Sphere Simulator
### 小行星軌道與天球互動模擬器

這是一個基於 **Three.js** 開發的互動式 Web 應用程式，旨在視覺化小行星在太陽系中的軌道運動，並同時展示其在天球上的觀測位置。

---

## 🌟 核心功能 (Key Features)

- **雙視角同步 (Dual View Synchronization)**:
  - **左側 - 太陽系視角 (Heliocentric View)**: 以 3D 方式呈現小行星與地球繞太陽運行的軌道。
  - **右側 - 天球視角 (Celestial Sphere View)**: 展示從地球觀測小行星時，其在星空中的座標位置。
- **即時軌道計算 (Real-time Physics)**: 基於開普勒定律與軌道根數（半長軸、偏心率、傾角等）進行精確模擬。
- **互動式操作 (Interactive Controls)**: 
  - 調整時間流逝速度與模擬步長。
  - 自定義小行星的軌道參數（$a, e, i, \Omega, \omega, M$）。
  - 支援繁體中文與英文介面切換。
- **詳細物理資訊 (Physical Data)**: 滑鼠懸停於數據區可查看公式（如週期 $T$、速度 $v$、重力位能 $E_p$ 等）。

## 🚀 線上展示 (Live Demo)

本專案已透過 GitHub Pages 發佈，你可以直接在瀏覽器中體驗：
👉 [https://xun73.github.io/asteroid_orbit/](https://xun73.github.io/asteroid_orbit/)

## 🛠️ 技術棧 (Tech Stack)

- **渲染引擎**: [Three.js](https://threejs.org/) (R128)
- **UI 框架**: [Tailwind CSS](https://tailwindcss.com/)
- **語言**: HTML5 / JavaScript (ES6+)

## 📂 檔案結構 (File Structure)

```text
asteroid_orbit/
├── index.html      # 主程式檔案 (請將 MPCorbit.htm 改名為此)
└── README.md       # 本專案說明文件
```

## 📖 如何在本地運行 (How to Run Locally)

1. 將本儲存庫 Clone 到本地：
   ```bash
   git clone https://github.com/xun73/asteroid_orbit.git
   ```
2. 進入資料夾並直接使用瀏覽器開啟 `index.html` 即可運行。

## 🧪 科學公式參考 (Scientific Formulas)

本程式包含以下天文物理計算：
- **軌道週期**: $T = 2\pi \sqrt{rac{a^3}{GM}}$
- **活力公式 (Orbital Velocity)**: $v = \sqrt{GM_\odot \left( rac{2}{r} - rac{1}{a} ight)}$
- **距離公式**: $r = rac{a(1-e^2)}{1+e \cos 
u}$

---

Developed by [xun73](https://github.com/xun73)
