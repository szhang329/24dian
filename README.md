# 🃏 24点游戏 / 24-Point Game

> 一个经典的24点数学游戏网页版，支持移动端与桌面端。  
> A classic 24-point math game web app, supporting both mobile and desktop.

---

## 中文

### 📖 简介

24点游戏是一款经典的数学益智游戏。系统随机给出4个数字，玩家需要通过加（`+`）、减（`-`）、乘（`×`）、除（`÷`）以及括号运算，将这4个数字各使用一次，使算式的结果等于 **24**。

### 🎮 游戏规则

| 规则 | 说明 |
|------|------|
| 🎲 **出题** | 每轮随机生成4个数字，系统自动验证有解后才出题 |
| ✍️ **作答** | 使用所有4个数字各一次，通过 `+ - × ÷ ( )` 组合运算得出 24 |
| 🎯 **机会** | 每题有 **3 次** 提交机会，用尽则游戏结束 |
| 💡 **求助** | 每位玩家有 **2 次** 求助机会，点击可查看一种正确答案 |
| ⭐ **积分** | 每答对一题 +10 积分，游戏结束时展示总积分 |

### 🎚️ 难度等级

| 难度 | 数字范围 | 说明 |
|------|---------|------|
| 🟢 **简单** | 1 ~ 36 | 数字偏小，容易凑出 24，适合新手 |
| 🟡 **正常** | 1 ~ 64 | 数字适中，有一定挑战性 |
| 🔴 **困难** | 1 ~ 99 | 大数较多，需要仔细思考组合方式 |

### 🛠️ 功能特性

- ✅ 自动验证题目有解（暴力搜索算法）
- ✅ 运算符一键输入键盘（`+ − × ÷ ( )`）
- ✅ 点击数字卡片自动填入数字
- ✅ 支持直接键盘输入算式
- ✅ 光标位置智能插入（点击或键盘均支持）
- ✅ 答题成功 / 失败音效反馈（Web Audio API 合成）
- ✅ 答对撒花星星特效 🎉
- ✅ 答错抖动动画
- ✅ 剩余机会、积分、提示次数实时显示
- ✅ 完全适配手机与电脑屏幕

### 🚀 在线试玩

👉 **[https://dc721ab6.pinme.dev](https://dc721ab6.pinme.dev)**

---

## English

### 📖 Introduction

The 24-Point Game is a classic math puzzle. The system randomly generates 4 numbers, and players must use addition (`+`), subtraction (`-`), multiplication (`×`), division (`÷`), and parentheses, each number exactly once, to arrive at **24**.

### 🎮 Game Rules

| Rule | Description |
|------|-------------|
| 🎲 **Puzzle** | 4 random numbers are generated each round; the system guarantees at least one solution exists |
| ✍️ **Answer** | Use all 4 numbers exactly once with `+ - × ÷ ( )` to equal 24 |
| 🎯 **Chances** | **3 attempts** per puzzle — running out ends the game |
| 💡 **Hints** | **2 hints** available per game — shows one correct solution |
| ⭐ **Score** | +10 points for each correct answer; final score displayed at game over |

### 🎚️ Difficulty Levels

| Difficulty | Number Range | Description |
|-----------|-------------|-------------|
| 🟢 **Easy** | 1 ~ 36 | Small numbers, easier to solve, great for beginners |
| 🟡 **Normal** | 1 ~ 64 | Moderate numbers, offers a fair challenge |
| 🔴 **Hard** | 1 ~ 99 | Large numbers, requires careful combination planning |

### 🛠️ Features

- ✅ Auto-validates puzzles (brute-force solver ensures solvability)
- ✅ Operator button keyboard (`+ − × ÷ ( )`) for easy input
- ✅ Click number cards to auto-insert into the expression
- ✅ Direct keyboard input also supported
- ✅ Smart cursor-position insertion (both click and keyboard)
- ✅ Sound effects via Web Audio API (success/fail/hint/card click)
- ✅ Star celebration animation on correct answer 🎉
- ✅ Shake animation on wrong answer
- ✅ Real-time display of score, hints, and remaining chances
- ✅ Fully responsive — works on mobile and desktop

---

### 🧠 Technical Notes

- **Solver algorithm**: Brute-force enumeration of all 4! permutations × 4³ operator combinations × 5 bracket structures — verifies `|result - 24| < 1e-9`
- **Sound effects**: Synthesized in real-time using the **Web Audio API** (no external audio files needed)
- **Stack**: Pure HTML + CSS + JavaScript single-page app (no frameworks or build tools)

---

### 📄 License

MIT
