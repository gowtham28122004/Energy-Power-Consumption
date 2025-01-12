# Energy Power Consumption Trend Analysis

This project analyzes energy consumption trends across multiple buildings, focusing on water, gas, and electricity usage. The dataset includes details about consumption rates, pricing, and building information. The objective is to identify patterns and insights to optimize energy usage.

---

## Dataset Description

### Sheets and Columns
1. **Energy Consumptions**:
   - `Date`: The date of the energy measurement.
   - `Building`: The building associated with the consumption data.
   - `Water Consumption`: Water usage in liters or gallons.
   - `Electricity Consumption`: Electricity usage in kWh.
   - `Gas Consumption`: Gas usage in cubic meters or BTUs.

2. **Rates**:
   - `Year`: The year of the pricing data.
   - `Energy Type`: Type of energy (Water, Gas, Electricity).
   - `Price Per Unit`: Cost per unit of the energy type.

3. **Building Master**:
   - `Building`: Building identifier.
   - `City`: City where the building is located.
   - `Country`: Country of the building.

---

## Data Relationships

### Key Creation
A composite key was created using `Year` and `Energy Type` to establish a relationship between the **Rates** and **Energy Consumptions** tables.

### Relationships
- **Energy Consumption** was connected to **Building Master** using the `Building` column.

---

## Operations Performed

### Data Modeling
- Established relationships between tables to create a cohesive data model.
- Enabled cross-table analysis.

### DAX Operations
Performed calculations to derive insights, such as:
- Total energy consumption per building.
- Monthly and yearly consumption trends.
- Cost analysis based on `Price Per Unit` and consumption values.

---

## Insights
- **Consumption Trends**:
  - Trends in water, gas, and electricity consumption across different buildings.
- **Cost Analysis**:
  - Cost trends by city, country, and energy type.
- **Energy Efficiency**:
  - Identification of high-energy-consuming buildings.

---

## How to Use
1. Clone the repository:
   ```bash
   git clone https://github.com/gowtham28122004/Energy-Power-Consumption.git
