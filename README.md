# Airline-Data-Management-and-Analysis-Using-Power-BI

This project focuses on analyzing and visualizing airline operations using Power BI to derive meaningful insights that enhance operational efficiency and customer satisfaction.

The airline industry handles massive amounts of complex data involving flights, passengers, and ticketing systems. Our goal is to transform this raw data into an interactive and insightful dashboard that helps stakeholders make informed decisions.

## Data Modeling

To ensure efficient querying and accurate reporting, we created a star schema model linking three key datasets:

    flight_information (Fact Table)

    ticket_information (Dimension Table)

    passenger_information (Dimension Table)

🔗 Relationships

    FlightID is used as the primary key to relate:

        ticket_information → flight_information

        passenger_information → flight_information

This structure tells the one to many relationship from flight_information to passenger_information and flight_information to ticket_information.

![Data Modeling](https://github.com/user-attachments/assets/60d2ca43-61c1-4a1b-a8ef-120cdee40a4b)

Enhanced Data Insights

In this step, we enriched the dataset to make insights more actionable and intuitive using Power BI's data transformation tools.
Key Enhancements:

Flight Performance Classification:
    A conditional column was added to classify flights as:

     Best – for flights with on-time or optimal Status.

     To Be Improved – for flights marked delayed, cancelled, or needing attention.

Flight Number Extraction:
    The FlightNumber column was split or transformed using "Column from Examples" to extract only the numeric flight number or airline code (depending on analysis needs).
    This supports better filtering, grouping, and normalization across visuals and calculations.
    
![image](https://github.com/user-attachments/assets/5a4ff3eb-d029-4304-a938-ddd5b8083837)

Final Dashboard

The final dashboard offers a consolidated, interactive view of key airline operations. It enables quick insights into passenger trends, booking status, flight performance, and route distribution.
Included Visuals:

    Summary Cards:

        🔢 Total Passengers

        🎟️ Total Tickets

        🆔 Total Flight ID

    Flight Performance Classification
    Bar chart displaying counts of flights marked as Best or To Be Improved.

    Passenger Count by Airline
    Horizontal bar chart to visualize how many passengers each airline serves.

    Ticket Booking Status
    Donut chart showing distribution of tickets by status: Confirmed, Pending, and Cancelled.

    Flights by Airline and Destination
    Stacked column chart showing the number of flights for each airline across destinations like Chicago, Houston, New York, etc.

    Interactive Slicers:

        ✈️ Airline Selector

        ⏱️ Flight Status

        🗺️ Destination Filter

![image](https://github.com/user-attachments/assets/0c3d450d-cfb8-45d0-89d7-ae9d8a1fe127)

