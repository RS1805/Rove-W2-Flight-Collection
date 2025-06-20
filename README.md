# Rove-W2-Flight-Collection
This project collects flight data from five major international routes using the Amadeus API. It stores the data in a local SQLite database and exports a clean Excel report for analysis. Ideal for developers, researchers, and students interested in aviation data.

---

## 🔍 Features

- Collects flight data for:
  - JFK → LAX
  - SIN → JNB
  - BOS → ZRH
  - YVR → SFO
  - YYZ → NRT
- Stores data in `flights_data.db` using SQLite
- Outputs Excel file `flight_data_July2025.xlsx`
- Includes flight details like:
  - Airline
  - Departure & arrival airports
  - Scheduled departure time
  - Price in USD
  - Number of layovers
- Supports `.env` configuration for API credentials

---

## 📁 File Structure

```
📂 Rove Flight Data Collection/
│
├── main.py                  # Main script to run everything
├── .env                     # Your Amadeus API keys (not uploaded to GitHub)
├── requirements.txt         # Python package dependencies
├── flights_data.db          # (Auto-generated) Database file
├── flight_data_July2025.xlsx # (Auto-generated) Excel export
```

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/rove-flight-data.git
cd rove-flight-data
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Set Up Your `.env` File

Create a `.env` file in the project root with your [Amadeus API](https://developers.amadeus.com) credentials:

```env
CLIENT_KEY=your_amadeus_client_id
CLIENT_SECRET=your_amadeus_client_secret
```

> 🔐 **Do not share your `.env` file publicly.**

---

### 4. Run the Script

```bash
python main.py
```

It will:
- Fetch data from Amadeus
- Store it in SQLite
- Export it to Excel


## 🛠 Dependencies

- `pandas`
- `amadeus`
- `python-dotenv`
- `xlsxwriter`

Install with:

```bash
pip install -r requirements.txt
```

---

