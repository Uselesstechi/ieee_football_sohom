# ieee_football_sohom(my_new_branch)

⚽ IEEE Football API – Sohom
A RESTful API designed to provide detailed football statistics and predictive analytics. This project was developed as part of the IEEE student chapter initiative.​

📌 Features

Retrieve comprehensive player statistics for specific seasons.

Access team details, including player rosters and performance metrics.

Fetch league standings and tables for various seasons.

Generate predictive analytics for league outcomes.​

🚀 Getting Started

Prerequisites
Python 3.7 or higher

pip package manager​

Installation

1 . Clone the repository:

bash

git clone https://github.com/Uselesstechi/ieee_football_sohom.git

cd ieee_football_sohom

2 . Create and activate a virtual environment (optional but recommended):

bash

python -m venv venv

source venv/bin/activate  # On Windows: venv\Scripts\activate

3 . Install the required dependencies:

bash

pip install -r requirements.txt

4 . Run the application:

bash

python app.py

The API will be accessible at http://localhost:5000/.

📚 API Endpoints

🔹 Get Player Statistics

Endpoint: GET /player

Description: Fetches statistics for a specified player and season.

Request Body:

json

  {
    "playerName": "L. Messi",
    "season": 19
  }
  
<< Response: Returns a JSON object containing various player attributes, such as:

attacking_crossing

attacking_finishing

club_name

dribbling

pace

...and more.​

🔹 Get Team Details

Endpoint: GET /team

Description: Retrieves information about a specific team, including its players and performance metrics.

Request Body:

json

  {
    "teamName": "FC Barcelona",
    "season": 19
  }
  
Response: Returns a JSON object with team statistics and a list of players.​

🔹 Get League Table

Endpoint: GET /table

Description: Provides the league standings for a specified league and season.

Request Body:

json

  {
    "league": "Spain Primera Division",
    "season": 19
  }
  
Response: Returns a JSON array detailing the positions of teams in the league.​

🔹 Predict League Outcomes

Endpoint: GET /predict

Description: Generates predictions for league standings based on historical data.

Request Body:

json

  {
    "league": "Spain Primera Division",
    "season": 19
  }
Response: Returns a JSON array with predicted points and rankings for each team.​

🧪 Example Usage

To fetch statistics for Lionel Messi in the 2019 season:​

bash

curl -X GET http://localhost:5000/player \
     -H "Content-Type: application/json" \
     -d '{"playerName": "L. Messi", "season": 19}'
     
🛠️ Technologies Used

Python 3.7+

Flask

Pandas

NumPy

Scikit-learn

SQLite (or another database if specified)​

📂 Project Structure

plaintext :-

ieee_football_sohom/
├── app.py

├── requirements.txt

├── README.md

├── models/

│   └── prediction_model.pkl

├── data/

│   └── players.csv

│   └── teams.csv

└── ... 

📄 License

This project is licensed under the MIT License. See the LICENSE file for details.​

🤝 Contributing

Contributions are welcome! Please fork the repository and submit a pull request for any enhancements or bug fixes.​

📬 Contact

For any inquiries or feedback, please contact sohombhowmick14@gmail.com.​
