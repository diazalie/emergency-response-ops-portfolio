
# Emergency Response Operations — Portfolio Project

## Executive Summary
The Emergency Response team manages traveler disruption cases worldwide.  
Using SQL in Snowflake, I cleaned and analyzed case data to uncover operational bottlenecks.  
Key findings:
- **Most cases are low urgency (Severity D/C)** → staffing should prioritize routine triage.  
- **Top 10 agents resolve cases in ~160–190 mins** → coaching opportunities for slower peers.  
- **Italy, U.S., and Japan generate the most cases (~190–200 each)** → need regional partnerships.  

## Business Problem
Case resolution speed directly impacts traveler safety and satisfaction.  
Leadership wanted visibility into:
1. **Severity mix** of cases (are we overstaffed/understaffed for critical cases?).  
2. **Agent performance** (who resolves fastest and why?).  
3. **Geographic hotspots** (where are disruptions most frequent?).  

## Methodology
- **SQL (Snowflake):**  
  - Standardized severity codes (A–D).  
  - Calculated case resolution minutes.  
  - Aggregated by severity, agent, and country.  
- **Visuals (Snowflake Notebook/Altair):**  
  - Bar charts, leaderboards, and country breakdowns.  
- **Business Storytelling:**  
  - Markdown summaries + action steps for each chart.  

## Skills
- SQL: Joins, aggregations, CASE/UPPER, DATEDIFF, view creation  
- Data Cleaning: standardizing categorical fields, handling nulls  
- Visualization: Altair bar charts, labeling, sorting  
- Business Communication: turning queries → executive summaries  

## Results & Business Recommendations

- **Severity mix:** Routine low-severity cases dominate → staff triage teams accordingly; maintain an escalation lane for Severity A/B.
![Cases by Severity](cases%20by%20severity.png)  
*Severity B and C cases dominate the workload, while Severity A cases require the fastest response times.*

- **Agent performance:** Fastest agents average ~3 hours; some are high-volume + fast → replicate workflows, coach slower peers, align shifts with top performers.
![Top 10 Agents](top%2010%20agents.png)  
*Top-performing agents resolve significantly more cases, highlighting opportunities for knowledge-sharing and workflow optimization.*

- **Geographic hotspots:** Italy, U.S., Japan show highest disruption volume → strengthen local provider partnerships, allocate more regional coverage, and add proactive traveler communication.
![Cases by Country](cases%20by%20country.png)  
*Distribution of cases shows the highest volume from North America and Europe, with notable clusters in Asia-Pacific.*

**Business Impact:**  
By aligning staffing, training, and regional partnerships with data, Emergency Response can reduce resolution times, improve efficiency, and enhance traveler experience.
