# CASE-004

---

# Document Information

| Field | Value |
|--------|-------|
| Case ID | CASE-004 |
| Working Title | Predictive Capacity Planning Model for Manufacturing Expansion |
| Company | Consorcio Geohidráulica S.A.C. |
| Position | Production & Maintenance Manager |
| Year | 2022 |
| Classification | Executive Case |
| Estimated Business Impact | Strategic |
| Status | Approved v1.0 |

---

# Executive Summary

The General Manager required an objective method to determine the real production capacity of a highly customized manufacturing operation in order to support future investments, plant expansion, and equipment acquisition decisions.

The manufacturing environment presented an exceptional level of complexity: multiple product families, thousands of spare parts, different machining routes, alternative machine assignments, internal manufacturing, outsourced operations, repair activities, and continuously changing demand.

Instead of attempting to calculate a static production capacity, I designed and developed a predictive mathematical model that transformed commercial demand forecasts into machine occupancy projections.

Built entirely in Microsoft Excel using data extracted from the company's databases, the model integrated production, maintenance, sales forecasts, equipment utilization, labor availability, efficiency, setup times, overtime, and future equipment acquisitions into a single decision-support tool.

The model achieved approximately 92% predictive accuracy and became the primary planning tool for expansion projects, machinery investments, production planning, and scenario simulation.

---

# 1. Business Context

Consorcio Geohidráulica manufactures specialized dewatering pumps used in underground mining operations.

Unlike conventional manufacturing environments, the company simultaneously managed:

- Production of new pumps.
- Maintenance of approximately 800 rental pumps installed in mining operations.
- Manufacturing of spare parts.
- Repair of customer-owned equipment.
- Internal motor rewinding.
- Electrical panel manufacturing.
- Continuous replenishment of strategic inventory.

Approximately 65 pumps returned weekly from mining operations for complete refurbishment while new pumps continued to be manufactured according to commercial demand.

As the company prepared for physical expansion, executive management required an accurate understanding of the plant's true production capacity in order to determine future investments and avoid creating new production bottlenecks.

---

# 2. Initial Situation

The company had no formal capacity planning model.

Calculating capacity was particularly difficult because:

- Components followed multiple machining routes.
- Individual parts could be processed on machines of different sizes.
- Larger machines could perform smaller jobs, but not vice versa.
- Production was organized in batches.
- Some machining operations were outsourced.
- Processing times varied according to material, size and product family.
- Production and maintenance activities competed for the same manufacturing resources.

The manufacturing system included:

- Eight pump power ranges with multiple product variants.
- Approximately 2,500 spare part references.
- Twenty-two production machines distributed across five different equipment categories.
- Components requiring between two and four machining operations before assembly.

Traditional capacity calculations were insufficient for representing this level of operational complexity.

---

# 3. Business Objective

Executive management required a reliable method to answer strategic questions such as:

- What is the actual production capacity of the plant?
- Which production areas will become future bottlenecks?
- When should additional machinery be purchased?
- How will future sales affect machine utilization?
- Which investments should be prioritized?

My objective was to transform a highly variable manufacturing system into a practical decision-support model capable of supporting investment planning under multiple business scenarios.

---

# 4. Root Cause Analysis

Rather than beginning with available production data, I started by defining the final business decisions the model needed to support.

This reverse-design approach allowed me to identify only the variables that genuinely influenced executive decision-making while deliberately excluding information that added complexity without improving prediction quality.

The conceptual structure became:

### Inputs

- Forecasted sales.
- Production of new pumps.
- Spare parts demand.
- Maintenance workload.
- Process efficiency.
- Overtime availability.
- New equipment acquisitions.

### Outputs

- Machine occupancy by equipment type.
- Capacity utilization.
- Future production bottlenecks.
- Expansion requirements.
- Investment timing.

To produce meaningful results, the model also incorporated:

- Available labor hours.
- Calendar constraints.
- Holidays.
- Setup times.
- Equipment efficiency.
- Machine substitution rules.
- Progressive replacement of conventional equipment by CNC machinery.

Instead of forcing deterministic values into an inherently variable system, I adopted statistically representative trends while removing anomalous observations from the historical data.

---

# 5. Executive Decision

The most important decision was accepting that a perfect model was neither achievable nor necessary.

Rather than attempting to eliminate all uncertainty, I focused on identifying reliable patterns that could support high-quality executive decisions.

A second key insight was recognizing that management and production viewed capacity through different units.

Management measured capacity in pumps delivered.

Operations measured capacity in available production hours.

The model successfully connected these two perspectives through the intermediate workload generated by each component throughout the manufacturing process.

---

# 6. Implementation

Historical operational data was extracted from the company's databases and consolidated into an integrated Excel model.

The solution included:

- Automated relationships between production databases and calculation sheets.
- Statistical filtering of inconsistent historical information.
- Estimation methods for incomplete data.
- Machine allocation logic.
- Capacity calculations by production area.
- Demand forecasting.
- Maintenance projections.
- Equipment occupancy calculations.

A dedicated front-end worksheet allowed executive management to modify planning variables without interacting with the underlying calculations.

Decision makers could instantly simulate different scenarios by adjusting variables such as:

- Sales forecasts.
- Process efficiency.
- Overtime utilization.
- Acquisition of new machinery.

The model automatically recalculated the expected utilization of every production resource.

Additionally, executive summary reports were generated for strategic presentations, while the interactive model allowed real-time simulation during management meetings.

---

# 7. Business Results

## Quantitative Results

- Developed the company's first integrated capacity planning model.
- Approximately 92% prediction accuracy.
- Twelve-month planning horizon.
- Weekly operational resolution.
- Integrated more than 2,500 spare part references.
- Modeled 22 production machines across five equipment categories.
- Supported production, maintenance, inventory, and expansion planning within a single analytical framework.

## Qualitative Results

Executive management gained a structured decision-support tool capable of evaluating multiple investment scenarios before committing capital.

The model transformed capacity planning from subjective estimation into a quantitative decision process.

## Strategic Results

The model became the foundation for:

- Machinery acquisition decisions.
- Plant expansion planning.
- Equipment replacement timing.
- Production planning.
- Workforce planning.
- Sales scenario evaluation.

Its ability to perform live simulations significantly improved executive discussions by allowing alternative investment strategies to be evaluated immediately during planning sessions.

---

# 8. Executive Impact

Beyond calculating production capacity, the project introduced a new planning capability within the organization.

Instead of reacting to production constraints after they appeared, management could anticipate future bottlenecks months in advance and align investments with projected business growth.

The model also facilitated communication between commercial, production, maintenance, and executive teams by providing a common quantitative framework for strategic planning.

---

# 9. Executive Thinking

This project reinforced one of my strongest engineering principles:

**In complex industrial systems, the objective is not to eliminate uncertainty, but to build models that are sufficiently reliable to improve strategic decision-making.**

Beginning with the desired business decision rather than the available data allowed me to simplify a highly complex manufacturing environment without sacrificing predictive accuracy.

By focusing on the variables that truly influenced capacity, I transformed operational complexity into an executive planning tool capable of supporting investment decisions with confidence.

---

# 10. Transferable Executive Knowledge

Complex manufacturing systems rarely require perfect mathematical representations.

They require practical models that capture the dominant variables affecting business performance while filtering out operational noise.

Effective executive models should prioritize decision quality over mathematical perfection.

Designing analytical systems from the desired business outcome backward enables organizations to concentrate on the information that creates value rather than attempting to model every operational detail.

This approach is applicable to capacity planning, supply chain design, production scheduling, maintenance forecasting, capital investment planning, and virtually any industrial environment characterized by high operational variability.

---

# 11. ATS Competencies

*To be developed as part of the Executive Career Portfolio competency mapping.*
