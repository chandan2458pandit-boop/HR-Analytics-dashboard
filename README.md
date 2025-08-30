# HR-Analytics-dashboard
The HR Analytics Dashboard shows 433 employees with 20.8% attrition (90 exits). Most attrition is among Sales Executives, employees aged 26–35, and those earning 5k–10k. Marketing and Life Sciences grads leave the most. Attrition peaks at 5 years of service and is higher among males.
Here’s a clear walkthrough of your HR Analytics dashboard (filtered to **Sales**):

## Executive snapshot

* **Total Employment:** 433
* **Attrition:** 90  → **Rate:** **20.8%**
* **Avg Age:** 36.6 | **Avg Salary:** 7.3 (unit per dataset) | **Avg Years:** 37 (tenure/YOE per dataset)
* **Gender mix (card):** Male 226, Female 166

## What the visuals show

* **Attrition by Salary:** Biggest exits in low bands—**5k–10k (201)** and **≤5k (158)**; falls sharply above 10k (44) and 15k+ (30).
  **Takeaway:** Pay bands under 10k are the churn hotspot.

* **Job Role (bars):** Headcount distribution—**Sales Executive 315**, **Sales Rep 82**, **Manager 36** (these sum to 433, so this visual is headcount, not attrition).
  **Attrition by JobRole × Satisfaction (matrix):** Exits = **Sales Exec 55**, **Sales Rep 33**, **Manager 2** across satisfaction levels **1–4**.
  **Takeaway:** Most attrition volume comes from Sales Executives.

* **Attrition by Year (line):** Spikes near **year 5 (\~55)** and **year 10 (\~37)**, troughs around years 12–14.
  **Takeaway:** Mid-tenure churn (especially \~5 years) is a key risk point—watch promotion/comp plans here.

* **Attrition by Education (donut):** **Marketing 37.62%**, **Life Sciences 34.78%**, **Medical 17.27%**, **Technical Degree 6.78%**.
  **Takeaway:** Leavers are concentrated in Marketing & Life Sciences backgrounds.

* **Attrition by Age (bars):** Highest in **26–35**, then **36–45**; very low **55+**.
  **Takeaway:** Early-mid career talent is most at risk.

## Actions you can take

1. **Compensation:** Review bands **≤10k**; introduce step-ups/variable pay for 3–6 year tenure.
2. **Role-specific:** Target **Sales Exec** with coaching, clear career paths, and quota fairness reviews.
3. **Tenure triggers:** Create stay-interviews at months/years linked to peaks (e.g., 48–60 months).
4. **Age/Education cohorts:** Tailor development tracks for 26–35 age band and Marketing/Life-Sci cohorts.
5. **Satisfaction:** Use the matrix to pinpoint low **JobSatisfaction (1–2)** cells by role and act there first.

## Quality notes (quick fixes)

* The **“Attrition by JobRole”** bar is actually **headcount**—rename or switch to an attrition measure.
* **“Attrition by Age”** axis shows **“Sum of Education”**—adjust to **Attrition Count** (e.g., `COUNTROWS` of leavers or a `[Attrition Count]` measure).
* Clarify units for **Average Salary** and **Average Year** in card titles.

If you want, I can give you DAX for **Attrition Rate**, **Attrition Count**, dynamic titles, and a corrected **Age** visual.
