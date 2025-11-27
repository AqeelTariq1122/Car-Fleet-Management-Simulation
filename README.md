# 🚗 Demand Point Model – Car Fleet Management Simulation

> A one-week AnyLogic simulation where cars respond to city-wide demand points, visit service stations, and generate data to improve fleet allocation and station utilization.

---

## 🧠 Project Overview

This model simulates a **small taxi fleet** operating in a city:

- **Cars are agents** that receive demand messages from destinations (offices, restaurants, groceries, malls).
- Each car chooses the closest demand point to serve and drives across a road network.
- Cars occasionally visit the closest **service stations**, where each station can serve **one car at a time** for **40 minutes**, with queues forming when busy.
- The simulation runs for **7 days** and records **trips, station usage, and queues**.

The goal is to find **better fleet positioning and station planning** using the data collected.

---

## 🎯 Impact Highlights

> Identify **high-demand areas** as measured by **number of taxi trips per demand point** by tracking how often each car visits offices, restaurants, groceries, and malls over a 7-day simulation.

> Valuable **service station optimization insights** as measured by **number of cars serviced and maximum queues per station** by modeling five stations with one-at-a-time service and 40-minute service times.

> Actionable **fleet reallocation recommendations** as measured by **uneven demand distribution (e.g., Grocery 1 vs Grocery 2)** by analyzing trips data and showing that some locations and stations can be scaled down while others should be reinforced.

---

## 📊 Key Results & Insights

### Demand Points (Trips by Taxi)

The stats dashboard shows how many times cars visit each destination.  
Examples from one week:

- **Grocery 1**: 20 visits  
- **Grocery 2**: 0 visits  
- **Office 1**: 8 visits  

➡️ This suggests **keeping more taxis near high-demand locations (like Grocery 1)** and reducing presence near no-demand points (like Grocery 2).

### Service Stations

Stations record **how many cars they serviced** and the **maximum queue length**.

- **Station 4**: Highest load – 6 cars serviced in 7 days, with queues forming.  
- **Station 3 & 5**: 0 cars serviced (idle for the entire week).

➡️ This supports decisions such as:
- **Closing or relocating Station 3 and Station 5**, and  
- **Adding capacity near Station 4**, where demand is consistently higher.

---

## 🛠️ Technologies & Tools

| Category        | Tools                |
|-----------------|---------------------|
| Simulation      | AnyLogic(DES & ABS)            |
| Modeling        | Agent-based cars, demand points, service stations |
| Analytics       | Trip counts, station utilization, queue metrics |
| Visualization   | City map animation, bar charts, stats dashboard |

---

## 🔄 Methodology

1. **Model demand points** (offices, restaurants, groceries, malls) on a city road network.
2. **Create car agents** that receive demand messages and travel to requested locations.
3. **Assign service stations** that handle one car at a time for 40 minutes, with queues.
4. **Run a 7-day simulation** and collect:
   - Trips to each demand point per car  
   - Service count and max queue per station  
5. **Analyze imbalances** in demand and station usage to recommend reallocation.

---

## 🖥️ How to Run

1. Open the model `.alp` file in **AnyLogic**.  
2. Choose **Animation** to watch cars move across the map, or **Stats/Charts** to see demand and station data.  
3. Run the simulation for the full 7-day horizon.  

---

## 🏁 Conclusion

This demand point model turns a simple taxi scenario into a **decision-support tool**:

- Shows **where taxis are actually needed** (high vs zero-demand points).  
- Highlights **underutilized stations** that can be closed or relocated.  
- Supports **better fleet positioning and infrastructure planning** to reduce costs and improve service.

---

## 👨‍💻 About the Author

**Aqeel Tariq**  
Operations Analyst | Simulation Modeling & Data Visualization  
AnyLogic ▪ Python ▪ Java ▪ Streamlit  
Focused on using digital models to improve real-world operations.
