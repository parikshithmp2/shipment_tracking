# shipment_tracking
This project processes shipment tracking data provided in JSON format, flattens the structure, computes key delivery metrics, and outputs clean CSVs for analysis.

# Input:
A JSON file containing shipment data with fields like:
- Tracking number
- Payment type (Prepaid/COD)
- Pickup/Delivery timestamps
- Pickup/Drop location
- Shipment weight
- Out for Delivery events

# Features:
- Converts all UTC timestamps to IST
- Calculates:
  - Days taken for delivery
  - Number of delivery attempts (handling same-day delivery edge cases)
- Outputs a clean, flat CSV file
- Generates summary statistics (mean, median, mode)

# Output:
- flattened_shipments.csv`: Flattened dataset
- summary_statistics.csv`: Summary metrics for delivery performance
