# Airbnb Seattle — Tableau Data Visualization Project

A Tableau workbook that explores the classic **Seattle Airbnb Open Data** dataset, analyzing listing prices, bedroom availability, and revenue trends across the city.

## 📊 Overview

This project connects Airbnb's Seattle listings, calendar, and review data to build a set of interactive visualizations covering pricing patterns, geographic price distribution, and revenue over time.

## 📁 Repository Contents

| File | Description |
|---|---|
| `AirBnB_Full_Project.twb` | Tableau workbook containing all worksheets and visualizations |
| `Tableau_Full_Project.xlsx` | Source data workbook (Listings, Reviews, Calendar) |

## 🗂️ Data

The underlying data source (`Listings+`) is built by joining the following tables from the Excel workbook:

| Sheet | Rows | Description |
|---|---|---|
| **Listings** | ~3,800 | Property details — host info, location, room type, price, amenities, review scores, etc. |
| **Calendar** | ~1M | Daily availability and price per listing across the calendar year |
| **Reviews** | ~84,800 | Guest reviews with reviewer, date, and comment text |

The Tableau workbook joins **Listings** and **Calendar** on `listing_id`/`id` to power price and revenue analysis.

## 📈 Visualizations

The workbook includes the following worksheets:

- **Distinct Count of Bedroom Listings** — count of unique listings broken out by number of bedrooms
- **Price Per Bedroom** — average nightly price by bedroom count
- **Price by Zipcode** — average nightly price by zip code
- **Price Per Zipcode** — filled map of Seattle showing average price by zip code (polygon/geo map)
- **Revenue for Year** — total revenue (sum of price from the calendar) trended by date

## 🛠️ Tools Used

- **Tableau Desktop** — workbook build and visualization
- **Microsoft Excel** — source data storage

## 🚀 Getting Started

1. Clone or download this repository
2. Open `AirBnB_Full_Project.twb` in [Tableau Desktop](https://www.tableau.com/products/desktop) or [Tableau Public](https://public.tableau.com/)
3. Keep `Tableau_Full_Project.xlsx` in the same relative location referenced by the workbook, or reconnect the data source if prompted (`Data > Edit Data Source Connection`)

## 📌 Data Source

Data originates from the [Inside Airbnb](http://insideairbnb.com/) / Seattle Airbnb Open Data collection, commonly distributed via [Kaggle](https://www.kaggle.com/datasets/airbnb/seattle).

## 📄 License

This project is for educational and portfolio purposes. Underlying Airbnb data is subject to its original source's license terms.
