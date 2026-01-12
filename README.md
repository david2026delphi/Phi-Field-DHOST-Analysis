# Φ-場拓撲幾何學：基於 Hessian 退化構造之最小 DHOST 原型分析
# (Topological Geometry of Φ-Field: Minimal DHOST Prototype Analysis)

[![arXiv](img.shields.io)](arxiv.org)
[![License: MIT](img.shields.io)](opensource.org)
[![Python 3.10+](img.shields.io)](www.python.org)

本儲存庫包含論文 **《Φ-場拓撲幾何學：基於 Hessian 退化構造之最小 DHOST 原型分析》** 的完整數學推導驗證與數值模擬代碼。

## 核心研究目標
本研究構造了一種最小化的退化高階標量-張量 (DHOST) 理論原型，旨在：
1. 驗證 Hessian 矩陣退化在規避 Ostrogradsky 幽靈模態中的關鍵作用。
2. 透過 Dirac-Bergmann 約束分析，嚴謹展示相空間如何縮約至單一物理自由度。
3. 證明該系統在強引力場模擬下具備高精度的數值穩定性（Hamiltonian 守恆達 $10^{-14}$）。

## 資料結構
*   `symbolic_derivation.py`: 基於 `SymPy` 的符號運算腳本，自動化計算：
    *   Lagrangian 的 Hessian 矩陣及其秩 (Rank)。
    *   共軛動量與初級、次級約束塔 ($\Phi_1$ 至 $\Phi_4$)。
    *   泊松矩陣 (Poisson Matrix) 的計算與分類。
*   `numerical_evolution.py`: 基於 `SciPy` 的數值模擬，驗證：
    *   系統的時間演化軌跡。
    *   哈密頓量 (Hamiltonian) 隨時間的守恆精度。
*   `requirements.txt`: 運行環境所需的依賴套件清單。

## 快速入門

### 環境準備
請確保您的環境已安裝 Python 3.10 或更高版本：
```bash
pip install -r requirements.txt
