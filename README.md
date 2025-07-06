Project Title:
Dynamic Pricing for Urban Parking Lots

Overview:
This project develops a real-time dynamic pricing engine for urban parking lots, aiming to optimize revenue and parking efficiency by adapting prices to fluctuating demand. The solution uses historical and real-time data, including occupancy, queue length, vehicle type, traffic, and special events, and applies a three-stage modeling approach to set optimal prices.

Project Structure:

File Name	Description
M1.ipynb	Baseline linear pricing model implementation.
M2.ipynb	Demand-based pricing model with multi-factor demand calculation.
M3.ipynb	Competition-aware pricing model with geographic adjustments.
dataset.csv	Main dataset with historical parking lot records.
parking_stream_m1.csv	Simulated real-time stream for Model 1.
parking_stream_m2.csv	Simulated real-time stream for Model 2.
parking_stream_m3.csv	Simulated real-time stream for Model 3.
ppt.pdf	Project presentation and methodology details.
README.md	Project overview and instructions.
Dataset Features:

Location: Latitude, Longitude for each lot (used for competition logic)

Capacity: Total vehicle holding limit

Occupancy: Current count of parked vehicles

Queue Length: Vehicles waiting to enter

Vehicle Type: Car, bike, or truck (affects pricing)

Special Event Indicator: Flags days with events or holidays

Traffic Conditions: Local congestion level

Timestamp: Date and time of each record

Models:

Model	Description	Key Features
M1	Baseline Linear Model	Price increases with occupancy ratio. Simple, transparent, scalable.
M2	Demand-Based Pricing	Multi-factor demand (occupancy, queue, traffic, events, vehicle type). Prices normalized and scaled.
M3	Competition-Aware Pricing	Adjusts price based on nearby lot prices and geographic proximity. Ensures competitiveness and fairness.
Tools & Technologies:

Python (main language)

Pandas, Numpy (data processing)

Pathway (real-time data streaming)

Bokeh (visualizations)

How to Use:

Review and run the Jupyter notebooks (M1.ipynb, M2.ipynb, M3.ipynb) in order to understand and simulate each pricing model.

Use the corresponding CSV files for each model to test real-time data streams.

Refer to ppt.pdf for project background, methodology, and results visualization.

Contact:
For questions or contributions, please refer to the project presentation or contact the project team.

For detailed formulas, assumptions, and visualizations, see ppt.pdf.
