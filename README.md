# AFCON 2025 Spectator Data Processor

A Spring Batch-based data processing pipeline to **validate**, **normalize**, and **analyze** spectator data collected during the 2025 Africa Cup of Nations in Morocco. The pipeline handles two source formats — JSON (from electronic gates) and XML (from other info systems) — with identical data semantics.

##  Features

- Import JSON and XML files  
- Validate schema and data consistency  
- Normalize data into a unified internal model  
- Perform data analysis (aggregations, stats)  
- Export or store processed data for reporting

##  Architecture

- **Source layer:** Reads JSON/XML from input directory  
- **Validation layer:** Validates structure & business rules  
- **Transformation layer:** Converts raw data into unified domain objects  
- **Batch processing:** Uses Spring Batch to orchestrate flows  
- **Analysis layer:** Runs summary computations, metrics, and aggregates  
- **Output layer:** Writes processed output (e.g., CSV, DB, or report)

##  Setup & Installation

1. Clone the repo:  
   ```bash
   git clone https://github.com/your‑username/afcon‑2025‑spectator‑data‑processor.git
