# Cricket Matches Assignment

This project interacts with a cricket data API to compute and display key statistics from recent cricket matches.

## Problem Statement

The task is to fetch cricket match data from an API and extract the following insights:

1. The highest score in a single innings, along with the team's name.
2. The number of matches where both teams had a combined score of 300 or more.

## API Information

The project uses the following API:

curl --location 'https://api.cuvora.com/car/partner/cricket-data'
--header 'apiKey: test-creds@2320'


The API returns JSON data for recent cricket matches, containing the following fields:

- **id**: Unique Match ID
- **dateTimeGMT**: Date and Time (GMT)
- **matchType**: Type of Match (T20, ODI, Test Match)
- **status**: Match Result (e.g., "Team A won by 10 runs")
- **ms**: Match Status (Result, Fixture, Ongoing)
- **t1**: Team 1 name
- **t2**: Team 2 name
- **t1s**: Team 1 score
- **t2s**: Team 2 score
- **t1img**: Team 1 Image URL
- **t2img**: Team 2 Image URL

## Features

- **Highest Score Computation**: The program computes the highest individual team score from the fetched matches.
- **Total 300+ Scores**: The program computes the number of matches where the total score from both teams exceeded 300.

## Setup Instructions

1. Clone the repository:
    ```bash
    git clone https://github.com/Mr-aj33t/Cricket_Match.git
    ```

2. Navigate to the project directory and ensure you have Java installed:
    ```bash
    cd Cricket_Match
    ```

3. Run the project:
    ```bash
    javac Main.java
    java Main
    ```

## Output

1. **Highest Score**: The highest team score in the data.
2. **300+ Total Score Matches**: Number of matches where both teams scored over 300 in total.


