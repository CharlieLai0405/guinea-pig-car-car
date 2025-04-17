# 🐹 Guinea Pig Car Car Race Simulation
A Java-based OOP simulation of a guinea pig car race with rule-driven behavior.

## Overview

This project simulates an annual race between three guinea pig cars — a police car, an ambulance, and a trash truck — using Java and object-oriented design. Each guinea pig car has its own name, vehicle type, speed, and behavior based on the rules defined in the assignment spec. The race proceeds second by second, with special behaviors triggered every 10 seconds. The first car to reach 4000 meters wins.

## Features

- 🏎️ 3 Vehicle types: PoliceCar, Ambulance, TrashTruck
- 🥕 Red carrot boosts speed, 🥬 lettuce has no effect
- 💩 When a car eats more than 5 food items, it "pupu" and resets speed
- 🏁 Real-time distance tracking and simulation logic
- ☑ Fully object-oriented: inheritance, polymorphism, encapsulation

---

## 內容說明

這是一個以 Java 開發的物件導向模擬專案，依據指定題目模擬三輛天竺鼠車車（警車、救護車、垃圾車）在跑道上進行比賽的行為：

- 根據車種決定初速度與加速度
- 每 10 秒最落後者吃紅蘿蔔（加速），最領先者吃生菜（不加速）
- 食物超過 5 個會自動棒賽（印出吃下的所有食物），並重設速度
- 比賽第一名一出現即結束，並印出所有選手的最終距離與冠軍名稱

---

## 📂 Project Structure

```
src/
├── Main.java
├── models/
│   ├── Car/
│   │   ├── Car.java
│   │   ├── PoliceCar.java
│   │   ├── Ambulance.java
│   │   ├── TrashTruck.java
│   │   └── CarType.java
│   ├── guineaPig/
│   │   └── GuineaPig.java
│   ├── GuineaPigCarCar.java
│   └── RunRunGuineaPigCarCarRace.java
```

---

## 🚀 How to Run

### 1. Compile

```bash
javac -d out $(find src -name "*.java")
```
> Windows PowerShell:
```powershell
javac -d out (Get-ChildItem -Recurse -Filter *.java -Path src | ForEach-Object { $_.FullName })
```

### 2. Run

```bash
java -cp out Main
```

---

## 💡 Example Output

```
阿比: 棒出了 lettuce, carrot, carrot, lettuce, lettuce, carrot
泰迪: 棒出了 carrot, lettuce, lettuce, lettuce, lettuce, carrot
西羅摩: 4022
阿比: 2370
泰迪: 1983
冠軍得主是:西羅摩
```

---

## 🔧 Techniques Used

- Java OOP Design: Inheritance, Polymorphism, Encapsulation
- CLI simulation logic
- Modular class structure
- Rule-driven game behavior

---

## 📌 Author

- Developed by Charlie Lai
- Institution: National Central University
