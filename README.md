# Citi Java Stock Price Simulation
A Java-based application developed as part of the Citi Technology Job Simulation.

The project demonstrates how a Java application can retrieve financial market data from an external API, process the data, store collected prices using a queue, and visualize price changes over time.

## Project Overview

The application retrieves DIA (SPDR Dow Jones Industrial Average ETF Trust) price data using the Twelve Data API.

During a single application run, the program:

1. Connects to the Twelve Data API.
2. Retrieves the current DIA price.
3. Records the timestamp and price.
4. Adds the collected data to a queue.
5. Repeats the process at regular intervals.
6. Uses the collected data to generate a line graph showing price changes over time.

## Technologies Used

- Java
- Google Colab
- Twelve Data API
- Python
- Matplotlib
- Git & GitHub
- REST API
- Queue Data Structure

## Project Structure

citi-java-stock-price-simulation/
│
├── App.java
├── dia_price_graph.py
├── Citi_Simulation.ipynb
├── screenshots/
└── README.md

## Data Flow

Twelve Data API
       ↓
   Java Application
       ↓
 Retrieve DIA Price
       ↓
 Timestamp + Price
       ↓
      Queue
       ↓
 Collected Data
       ↓
 Python + Matplotlib
       ↓
   Price Graph

## Example Output

The application collects data similar to:

Timestamp: 2026-09-24 12:00:00
DIA Price: $460.25

Timestamp: 2026-09-24 12:00:15
DIA Price: $460.31

Timestamp: 2026-09-24 12:00:30
DIA Price: $460.18

## Visualization

The collected data is visualized using Matplotlib.

- X-axis: Timestamp
- Y-axis: DIA Price

The graph provides a simple visual representation of how the DIA price changed during the application run.

## Key Skills Demonstrated

- Java programming
- API integration
- HTTP requests
- JSON data handling
- Queue-based data processing
- Environment-variable based API-key management
- Data collection
- Data visualization
- Debugging
- Git/GitHub version control

## Security Considerations

The Twelve Data API key is not stored directly in the source code.

The application retrieves the API key through an environment variable:

TWELVE_DATA_API_KEY

This prevents sensitive credentials from being exposed in the GitHub repository.

## Learning Outcome

This project provided practical experience connecting a Java application to an external financial API, processing real-time-style market data, managing collected data using a queue, and visualizing the resulting dataset.

## Author

Oluwadamilare Ojo

Software Developer | Cybersecurity Analyst | Computer Science Student | Graphic Designer

GitHub: https://github.com/Yoggys-Graph

Portfolio: https://yoggys-graph.github.io/Dre-Portfolio/
