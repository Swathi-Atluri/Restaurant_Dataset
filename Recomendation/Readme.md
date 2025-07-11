# Restaurant Recommendation System

Welcome to the Restaurant Recommendation System!  
This tool helps you discover the best restaurants based on your preferences — cuisine, city, locality, and budget.  

---

## Features

- Search by **Cuisine** (e.g., Japanese, North Indian, Bakery)
- Filter by **City**
- Optional filter by **Locality**
- Choose your **Price Range** (1: low budget to 4: premium)
- Accurate **Aggregate Ratings** (formatted to 1 decimal place)
- Prices displayed clearly with **Currency**

---

## How It Works

1. The system reads restaurant data containing cuisines, locations, prices, and ratings.
2. You enter your preferences:
   - Preferred **Cuisine** (or type `'Any'` to see all cuisines)
   - Your **City**
   - Your **Locality** (or type `'Any'`)
   - Preferred **Price Range** (1 to 4) or type `'Any'`
3. The system filters and recommends the **Near-by matching restaurants**.
4. Output is displayed in a clear and readable table format.

---


## Sample output:

| Restaurant Name  | Locality         | City         | Cuisines  | Price for 2  | Aggregate rating |
|------------------|------------------|--------------|-----------|--------------|------------------|
| Izakaya Kikufuji | Legaspi Village  | Makati City  | Japanese  | PHP 1200     | 4.5              |

---

## Data Requirements

Your data file (`df`) should include **these columns** exactly (case sensitive):

- `Restaurant Name`
- `Locality`
- `City`
- `Cuisines`
- `Average Cost for two`
- `Price range`
- `Aggregate rating`
- `Currency`

---

## Why This Stands Out

- Handles **case-insensitive** searches so user input always matches correctly
- Rounds restaurant ratings to **1 decimal place** for clean display
- Prices are displayed with the appropriate **currency symbol**
- Offers flexibility by allowing `'Any'` input for broad searches


