# GTFS Analytics Report

**Objective**

The goal of this project is to identify high‑impact transit patterns across York Region Transit (YRT) and Brampton Transit by analysing GTFS (General Transit Feed Specification) schedule data. This analysis can help in understanding service performance, which can be leveraged for operational insights, route comparisons, and improving rider experience. 

**Problem Statement:**

The analysis is structured around three guiding questions, each designed to move from system-level performance toward route-level decision support, ultimately informing targeted recommendations for service enhancement within York Region.

- **Which stops are served most frequently during weekday peak hours?**
- **Which routes operate with the longest and shortest service spans?**
- **How does a route progress through its stop sequence during peak periods?**

---

**Analysis**

**Visualizations and Their Purpose**

1. **Overview Dashboard**
    - **Metrics**: Total Arrivals, Distinct Routes, Distinct Stops
    - **Purpose**:
        - Provides a high-level **scale** of each transit system
        - This visual identifies major hubs and high‑demand locations.
2. **Top 20 Most Frequent Stops**
    - **Metrics**: stop_name, arrival_count.
    - **Visualizations**:
        - Horizontal bar chart showing the busiest YRT and Brampton transit stops by arrival count.
    - **Purpose**:
        - This visual identifies major hubs and high‑demand locations.
3. **Bus Routes by Service Span Duration (Top/Bottom 5)**
    - **Metrics**: service_span_hours, route_id
    - **Visualizations**:
        - Bar chart with toggle buttons showing longest and shortest service spans.
    - **Purpose**:
        - Monitor individual bus performance trends to provide actionable insights
        - Reveals operational extremes and highlights service coverage differences.
4. **Stop Sequence & Arrival Timing (Peak Period Route Spotlight)**
    - **Metrics**: stop_id, arrival_time, stop_name, stop_sequence
    - **Visualizations**:
        - Scatter plot showing how a selected YRT route progresses through its stops during peak time
        - Scatter plot showing the Brampton route movement during peak time. This mirrors the YRT version but uses Brampton’s stop sequence.
    - **Purpose**:
        - Identifies how the two agencies’ route spotlight visuals appear side‑by‑side or in sequence.
        - It visualizes movement along the corridor and the timing pattern of a single trip.

---

**Results**

The analysis revealed five distinct customer segments

**Key Findings**

1. From November 2025 to December 2025, YRT recorded **986,785** total arrivals across **124 distinct routes** and over **4,700 distinct stops.**
2. From November 2025 to December 2025, Brampton Transit recorded **1,048,575** total arrivals across **73 distinct routes** and over **2,900 distinct stops.**
3. **Frequency Increases:** Analysis highlights that Route 107 stops consistently rank in the Top 20 for frequency, with heavy transfer activity concentrated at the Keele and Jane nodes.
4. **Strong service intensity:** Route 107 demonstrates a strong overall service span, ranking second among YRT bus routes in our analysis, indicating effective all-day and late-evening coverage along the Keele corridor.
5. **Qualitative data:** Community feedback indicates a desire for “improved service span,” which may not reflect deficiencies in the main Route 107 service but could instead point to unmet demand for faster, limited-stop service outside peak periods and the creation of a much-needed "last-mile" link to GO Transit rail services.

---

**Conclusion**

Conducted a transit data analysis project using GTFS (General Transit Feed Specification) schedule files from York Region Transit (YRT) and Brampton Transit. Worked independently for two months, applying data preprocessing techniques, visualising key features, and investigating service patterns across stops, routes, and trips. Utilised SQL to extract high-impact segments and identify peak-hour performance. Developed visualisations to clearly present comparative insights across both systems. The goal is to identify actionable opportunities that align rider needs with operational realities

---

**Repository Contents**

- **Power BI File**:
    - `.pbix` file containing the dashboards and analysis.
- **Dataset**:
    - Dataset for reference.
- **README**:
    - Detailed documentation of the project, including objectives, analysis, results, and conclusions.
