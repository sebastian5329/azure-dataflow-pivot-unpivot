*Azure Data Factory – Pivot & Unpivot Data Flow*

*Project Overview*

This project demonstrates the implementation of Pivot and Unpivot transformations using Azure Data Factory Mapping Data Flows. It addresses a common data engineering scenario where multiple transactional records exist for the same entity and must be reshaped for analytical and downstream processing.

The transformations reflect patterns commonly used in reporting and analytical data preparation. The implementation is purposefully scoped to emphasize transformation behavior and orchestration patterns rather than complex business logic.

*What This Project Demonstrates*

	•	Handling multiple records per key (person and card type)
	•	Consolidating values using a Pivot transformation
	•	Restoring a normalized structure using Unpivot
	•	Building modular data flows and orchestrating them through pipelines
	•	Using a master pipeline for controlled execution

*Solution Design*

	•	Data Flow 1 (Pivot)
    Aggregates multiple credit score entries and pivots card types (Master, Visa) into columns.
	•	Data Flow 2 (Unpivot)
    Converts pivoted card-type columns back into rows and filters valid records.
	•	Pipelines
    Independent pipelines for Pivot and Unpivot transformations, orchestrated by a master pipeline to ensure sequential execution.

*Tech Stack*

	•	Azure Data Factory
	•	Mapping Data Flows
	•	Azure Data Lake Storage

*Purpose*

This project was built to practice and demonstrate data reshaping patterns commonly used in real-world ETL workflows, with a focus on clean design, reusability, and orchestration best practices.
