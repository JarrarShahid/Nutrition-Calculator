# 🥗 Calorie & Nutrition Calculator

![Python](https://img.shields.io/badge/Python-3.x-blue.svg)
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)
![Status](https://img.shields.io/badge/Status-Active-brightgreen)
![Platform](https://img.shields.io/badge/Platform-Cross--Platform-lightgrey)

A Python-based nutritional calculator built for a Health and Leisure company's app. This tool helps users estimate the total nutritional content calories, fats, sugars, protein, and carbohydrates of their food intake based on user input and a provided dataset.

---

## 📌 Project Overview

This feature was developed to empower users to make informed dietary choices by calculating nutritional values from a given dataset. It processes food entries and quantities, computes per-nutrient values, and returns a total nutritional summary.

---

## 📂 Dataset: `nutrition.json`

The dataset contains nutritional information per 100 grams of various food items. It's preloaded and parsed into a Python dictionary (`nutrition_dict`) for usage.

### 🧾 Sample Format

```json
{
  "Cornstarch": {
    "calories": 381,
    "total_fat": 0.1,
    "protein": 0.26,
    "carbohydrate": 91.27,
    "sugars": 0.0
  },
  ...
}
```

### 📊 Columns Description

| Key           | Description                                |
|---------------|--------------------------------------------|
| `calories`    | Energy in kcal per 100 grams               |
| `total_fat`   | Fat content in grams per 100 grams         |
| `protein`     | Protein content in grams per 100 grams     |
| `carbohydrate`| Carbohydrates in grams per 100 grams       |
| `sugars`      | Sugar content in grams per 100 grams       |

---

## ⚙️ How It Works

The `nutritional_summary()` function takes a dictionary of food names and gram values as input. It then:

1. Verifies if each food exists in the dataset.
2. Calculates the total nutritional values for each nutrient based on weight.
3. Returns a dictionary with the overall nutrient breakdown.

### 🧪 Example Input

```python
food_input = {
    "Croissants, cheese": 150,
    "Orange juice, raw": 250
}
```

### ✅ Example Output

```python
{
  'calories': 733.5,
  'total_fat': 32.0,
  'protein': 15.55,
  'carbohydrate': 96.5,
  'sugars': 38.03
}
```

---

## 🧠 Tech Used

- Python 3
- JSON for data storage
- Dictionary manipulation for calculation

---

## 🚀 Getting Started

1. Clone the repo.
2. Ensure `nutrition.json` is in the same directory.
3. Run the script using Python:
   ```bash
   python nutrition_calculator.py
   ```

---


## 🧑‍💻 Author

Built by a Software Engineer who enjoys creating useful tools that help people.

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.
