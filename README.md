# ☕ Coffee Vending Machine Analytics

Полный аналитический проект по данным кофейного автомата за **2024–2025 год** - от визуального дашборда до прогнозирования временных рядов.

Датасет: [Kaggle - Coffee Vending Machine Transactions](https://www.kaggle.com/datasets/ihelon/coffee-sales)

---

## Модули

### 📊 [dashboard/](dashboard/README.md)
Разведочный анализ и бизнес-дашборд. KPI-плитки, динамика выручки, популярность напитков, тепловая карта, способы оплаты, топ-клиенты, retention.
Палитра: **Espresso Dark** (`#1C0F08` фон).

<img width="1570" height="649" alt="heatmap" src="https://github.com/user-attachments/assets/c32075dd-1a4d-4c07-91e4-97c446e1adc8" />


### 📈 [time-series/](time-series/README.md)
Анализ временных рядов и прогнозирование. STL-декомпозиция, ACF/PACF, SARIMA, Prophet, сравнение моделей, обнаружение аномалий.
Палитра: **Flat White** (`#FAF3EB` фон).

<img width="1749" height="1338" alt="revenue" src="https://github.com/user-attachments/assets/38e6f0eb-6bde-42ae-9ccb-2c13aa8f8112" />


---

## Структура репозитория

```
coffee-dashboard/
├── dashboard/
│   ├── coffee_dashboard.ipynb
│   └── README.md
├── time-series/
│   ├── time_series.ipynb
│   └── README.md
├── data/                  ← положи CSV сюда (в git не попадают)
│   └── .gitkeep          
├── requirements.txt
├── .gitignore
├── LICENSE
└── README.md
```

---

## Быстрый старт

```bash
git clone https://github.com/Aisdz/coffee-dashboard.git
cd coffee-dashboard
pip install -r requirements.txt
```

Скачай датасет с Kaggle, положи `index_1.csv` и `index_2.csv` в `data/`, затем открывай нужный ноутбук.

---

## Требования

```
python >= 3.10
pandas, numpy, matplotlib, seaborn
statsmodels >= 0.14, prophet >= 1.1, scipy >= 1.11
```

Полный список - в [`requirements.txt`](requirements.txt).

---

## Рекомендации по улучшению

- Оценка точности моделей (MAE, RMSE, MAPE) на holdout-выборке
- Автоподбор параметров SARIMA через `pmdarima.auto_arima`
- Внешние регрессоры в Prophet (погода, праздники)
- Интерактивная версия дашборда на Plotly / Streamlit
- Мультимашинный анализ при расширении парка автоматов

---

## Лицензия

[MIT](LICENSE)
