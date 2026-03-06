# 🎲 蒙地卡羅模擬：馬可夫不等式之實證分析

本專案運用 **R 語言**與**蒙地卡羅模擬**，針對多種機率分配進行大規模隨機抽樣 (n=10,000)，旨在視覺化並實證機率論中的核心定理：**馬可夫不等式**。

## 👥 專案開發與協作聲明
本專案為統計模擬課程之期末小組專題，由本人與團隊成員共同研發。

## 🌟 專案與核心邏輯
馬可夫不等式指出，對於非負隨機變數 X 與常數 a > 0，其尾部機率滿足：**P(X ≥ a) ≤ E[X]/a**。
為了驗證此理論邊界，實作了以下模擬流程：
1. **多樣化分佈抽樣：** 涵蓋 Exponential, Normal, Half-Normal, Gamma, Chi-square, Lognormal, Beta, Uniform, Weibull 等 9 種連續型機率分配。
2. **蒙地卡羅實證：** 透過大樣本隨機生成，計算出Empirical Probability `mean(X >= a)`。
3. **動態視覺化對比：** 實作自定義比較函數，利用 R Base Plot 繪製理論上限 (Markov Bound)、模擬機率與兩者差值的動態關係圖，直觀證明定理之恆真性。

## 📂 檔案說明
* `Stat_Sim_Final_project.Rmd`: 包含隨機抽樣生成、期望值計算與繪圖函數之 R 程式碼。
* `統計模擬期末報告.pdf`: 模擬結果之圖表輸出與分佈特性分析報告。

## 🛠️ 開發環境
* **語言:** R
* **核心技術:** Monte Carlo Simulation, Probability Theory, Base R Graphics
