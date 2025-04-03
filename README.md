## ✈ Flight Deal Finder<br>
📌 Project Overview
Flight Deal Finder is an automated system that helps users find the best flight deals by tracking prices and sending alerts when prices drop below a certain threshold. It integrates with Google Sheets, Amadeus API, and Twilio to fetch flight details and notify users via SMS or WhatsApp.

🛠 Features
Retrieves flight price data from Google Sheets.

Uses Amadeus API to search for the best flight deals.

Updates missing IATA codes for destination cities.

Sends notifications via SMS and WhatsApp when a cheaper flight is found.

🚀 How It Works
The Google Sheet contains a list of destinations and their lowest recorded prices.

The system fetches this data and searches for cheaper flights using the Amadeus API.

If a cheaper flight is found, an SMS/WhatsApp alert is sent via Twilio.

The system updates the Google Sheet with new flight prices and IATA codes if necessary.

📂 Project Structure
main.py – Main script that coordinates data fetching, flight searching, and notifications.

data_manager.py – Handles interactions with Google Sheets via Sheety API.

flight_data.py – Processes and identifies the cheapest flights.

notification_manager.py – Manages SMS and WhatsApp notifications via Twilio.

.env – Stores sensitive API keys and credentials (not to be shared publicly).

🔧 Setup and Installation
Prerequisites
Python 3.x

Required libraries: requests, twilio, python-dotenv

Twilio and Amadeus API accounts.
