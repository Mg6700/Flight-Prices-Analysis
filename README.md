# Flight Prices Analysis — India Domestic Routes

**Tools:** Power BI, DAX  
**Domain:** Travel Analytics | Pricing Strategy | Consumer Insights  
**Portfolio:** [mg67.vercel.app](https://mg67.vercel.app/) | **GitHub:** [Mg6700](https://github.com/Mg6700)

---

## Project Overview

This project analyzes domestic flight pricing data across major Indian airlines and routes to uncover what drives ticket prices — departure time, days to travel, number of stops, airline, travel class, and route. The dashboard answers practical questions for travelers and provides strategic insights for pricing analysis, making it relevant for both consumer decision-making and airline revenue management contexts.

---

## Dashboard Preview

<img width="985" height="572" alt="image" src="https://github.com/user-attachments/assets/e6e87b4f-b7d1-4b07-844d-b504ca49b77c" />

---

## Dataset

| Field | Description |
|---|---|
| Airlines | Vistara, Air India, SpiceJet, GO FIRST, IndiGo, AirAsia |
| Cities | Bangalore, Chennai, Delhi, Hyderabad, Kolkata, Mumbai |
| Routes | All major metro-to-metro combinations |
| Features | Price, Departure Time, Days Left to Travel, Stops, Class (Business/Economy) |
| Source | Kaggle — Indian Flight Price Dataset |

---

## Key Metrics

| Metric | Value |
|---|---|
| Average Flight Price | ₹20,890 |
| Total Direct Flights Analyzed | 36,000 |
| Most Expensive Airline | Vistara (avg ₹30K) |
| Best Value Airline | AirAsia (avg ₹4K) |
| Highest Traffic Route (Direct) | Delhi–Mumbai / Mumbai–Delhi (₹3,600 avg) |

---

## Dashboard Features

- **Source City filter** — select origin city (Bangalore/Chennai/Delhi/Hyderabad/Kolkata/Mumbai)
- **Destination City filter** — select destination city
- **Average Flight Price by Airline** — horizontal bar ranking all 6 airlines by average price
- **Highest Direct Flight Routes** — top metro-to-metro routes ranked by direct flight price
- **Best Value for Money** — ranking airlines by price-to-value ratio
- **Relation b/w Flight Prices & Days Left** — scatter plot showing price vs booking lead time
- **Relation b/w Flight Prices, Departure Time & Class** — Business vs Economy price by time of day
- **Relation b/w Flight Prices & Stops** — scatter showing price impact of 0/1/2 stops
- **Relation b/w Flight Prices & Departure Time** — line chart of average price by departure slot

---

## Airline Price Comparison

| Airline | Average Price |
|---|---|
| Vistara | ₹30,000 |
| Air India | ₹24,000 |
| SpiceJet | ₹6,000 |
| GO FIRST | ₹6,000 |
| IndiGo | ₹5,000 |
| AirAsia | ₹4,000 |

**Best Value for Money (price-per-unit-quality):**
AirAsia (₹0.7K) → GO FIRST (₹0.8K) → SpiceJet (₹1.0K) → IndiGo (₹1.2K) → Air India (₹2.2K) → Vistara (₹3.1K)

---

## Top Direct Flight Routes

| Route | Average Direct Price |
|---|---|
| Delhi–Mumbai | ₹3,600 |
| Mumbai–Delhi | ₹3,600 |
| Bangalore–Delhi | ₹2,200 |
| Delhi–Bangalore | ₹2,200 |
| Mumbai–Bangalore | ₹1,600 |
| Bangalore–Mumbai | ₹1,600 |

---

## Key Findings

**1. Book early — prices drop sharply beyond 20 days in advance**
The scatter plot of Price vs Days Left shows a clear negative relationship — flights booked 20–50 days ahead cost significantly less than last-minute bookings. The trend line shows prices nearly double within the last 5 days.

**2. Late Night flights are the cheapest departure slot (avg ₹9,300)**
Departure time has a major impact on price. Late Night (avg ₹9,300) and Afternoon (avg ₹18,200) slots are cheapest, while Morning and Night slots average ₹20,000–₹21,600. Early Morning (₹21,200) offers mid-range pricing.

**3. Business class pricing is consistently elevated regardless of departure time**
The Business vs Economy scatter by departure time shows Business class prices clustering 3–5x above Economy across all time slots — confirming class is a stronger price driver than departure time for premium travelers.

**4. More stops = higher price (counter-intuitive finding)**
The stops scatter plot shows a positive relationship between number of stops and price — 1–2 stop flights cost more on average than direct flights. This likely reflects longer travel times and premium connection routes being priced higher, not lower.

**5. Vistara charges a 6x premium over AirAsia for comparable routes**
Vistara's ₹30K average vs AirAsia's ₹4K reveals a massive price spectrum in Indian domestic aviation — driven by service quality, seat comfort, and brand positioning.

**6. Delhi–Mumbai is the highest-priced direct route (₹3,600)**
The busiest business corridor in India commands the highest direct flight price — reflecting demand-driven pricing on India's most traveled domestic route.

---

## Practical Takeaways for Travelers

| Situation | Recommendation |
|---|---|
| Budget travel | AirAsia or GO FIRST, book 30+ days ahead, choose Late Night departure |
| Business travel | Vistara or Air India, Morning or Night slots for peak-hour connectivity |
| Best price on Delhi–Mumbai | Book 3+ weeks ahead, Late Night departure, IndiGo or SpiceJet |
| Avoiding price spikes | Never book within 5 days — prices jump sharply in final week |

---

## Technical Highlights

- Source and Destination city cross-filter enabling any route-specific analysis
- Scatter plots with trend lines for continuous variable relationships (days, stops, time)
- Business vs Economy overlay on departure time scatter for class comparison
- Airline ranking visuals with dynamic filtering
- DAX measures for average price calculations across multiple dimension combinations

---

## How to Use

1. Clone or download the repository
2. Open the `.pbix` file in Power BI Desktop (or view the PDF for a static preview)
3. Select **Source City** and **Destination City** to analyze a specific route
4. Review the scatter plots for pricing patterns by booking lead time, stops, and departure slot
5. Use the airline bar charts to compare price vs value across carriers

---

*Created by Mayur Goyal | [Portfolio](https://mg67.vercel.app/) | [LinkedIn](https://www.linkedin.com/in/mg67)*
