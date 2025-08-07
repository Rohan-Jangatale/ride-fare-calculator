# Distance-Based Ride Pricing

This Python module calculates the ride fare based on the geographical distance between a pick-up and drop location, with variable pricing depending on the time of booking.

---

## 🚀 Features

- Calculate the distance (in kilometers) using GPS coordinates (latitude, longitude).
- Time-based dynamic pricing:
  - ₹20/km during morning peak hours (9 AM to 11 AM)
  - ₹15/km during evening peak hours (7 PM to 9 PM)
  - ₹10/km during all other hours
- Returns the final price rounded to two decimal places.

---

## 🧠 How It Works

1. **Distance Calculation**: Uses the `geopy` library to calculate the geodesic distance.
2. **Dynamic Pricing**: Applies a price rate per kilometer based on the hour of the booking.
3. **Final Fare**: Multiplies distance by the price per kilometer and rounds it off.

---

## 🛠️ Requirements

Install the required package:

```bash
pip install geopy
