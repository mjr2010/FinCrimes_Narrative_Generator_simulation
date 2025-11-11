**🕵️‍♂️ FinCrimes Narrative Generator**

AI-Driven Financial Crime Case Analyzer and Narrative Generator
📘 **Overview**
FinCrimes Narrative Generator is a machine-learning and LLM-powered prototype that simulates how banks analyze and narrate suspicious financial activity using synthetic EFTR and SWIFT transaction data.
It aggregates raw transactions into case-level summaries, applies rule-based and ML risk scoring, detects structuring patterns, finds similar cases, and generates professional AML narratives automatically.

⚙️ **Key Features**
Synthetic Data Generator – creates customers, accounts, and transactions (EFTR, SWIFT, domestic).
Case Aggregation – groups transactions per account → calculates totals, counts, and unique countries.
Rule-Based Labelling – flags risky behavior (e.g., near-threshold EFTR, multiple SWIFT corridors).
Machine Learning Risk Model – RandomForest predicts risk level (High/Medium/Low).

**Advanced Analytics:**
Structuring pattern detection
Similar case search (cosine similarity)
Transaction timeline visualization

**Narrative Generation:**
Template-based case summary
LLM-based narrative using OpenAI API
Visual Outputs: correlation heatmap, feature importance chart, and timelines.

📈** Visual Outputs**
correlation_heatmap.png
feature_importance.png
transaction_timeline.png
Generated LLM narratives in CSV

🧩 **Example Use Case**
A customer sends multiple EFTR transfers just below $10,000 within 5 days and several SWIFT wires to different countries.
The system:
Flags RULE_STRUCTURING_EFTR_HIGH_VOLUME and RULE_SWIFT_MULTIPLE_CORRIDORS.
Assigns High Risk via the ML model.
Finds similar historical cases.
Generates an LLM-based narrative summarizing the findings.

🔮** Future Enhancements**
Add graph-based counterparty network analysis (Neo4j).
Introduce anomaly detection (Isolation Forest / AutoEncoder).
Generate regulator-ready SAR/STR drafts (FINTRAC-style).
Connect to open AML typology datasets for realism.

👤** Author**
Manasi Rane
