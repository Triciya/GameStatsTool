# Important information

On May 23, Valve released the major patch 7.39, which caused the website's database to be reset. If you notice a lot of missing data, please use the database file from May 17 located in the root resource folder.

# GameStatsTool

## About

GameStatsTool is a small program for extracting statistical data from a popular Dota 2 stats website.
The extracted data includes recommended item builds and skill sequences, based on the analysis of many matches played by highly skilled players.

Data is fetched using the GSON library, sorted, and stored locally in an SQLite database file.

## How to Use

1. Download and run the program.  
2. Click the **Update Database** button to fetch the latest data.  
3. (Optional) Click **Select Directory** to choose where database files are stored. By default, the database is placed in the program’s root folder.  
   > The **Select Directory** button also lets you open an existing database file if you want to compare previous data with the latest.  
4. After the database is updated, type a hero name into the input field to query statistics.

## Displayed Content

### Item Build

1. **Starting Items**  
   The initial items a player should buy at the start of a match. The purchase rate (as a percentage) helps inform decisions.

2. **Core Items**  
   The most commonly purchased, must-have items throughout the match.

3. **Early / Mid / Late Items**  
   Three sets of items, both situational and core, recommended for each phase:
   - Early (00:00–12:00)  
   - Mid (12:00–35:00)  
   - Late (35:00+)

### Skills

1. **Skill Learning Order**  
   A sequence of skill icons arranged by learning order.

2. **Talent Tree**  
   Recommended talent the recommended talent choices at each talent tier (levels 10, 15, 20, and 25).

## Additional Information

### Prerequisites

- Java Development Kit (JDK) 21
