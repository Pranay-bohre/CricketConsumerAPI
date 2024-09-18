# Cricket Match Data API Project

### Created by: **Pranay Bohre**

## Project Overview
This Java project is focused on consuming a cricket match data API to extract and compute useful match statistics. The project demonstrates how to retrieve and analyze cricket match data, performing calculations such as:

1. **Finding the Highest Score** in a single innings along with the team name.
2. **Counting the Number of Matches** where the total score from both teams exceeds 300.

### External JARs Used
To achieve these functionalities, we have integrated several external libraries that make it easy to handle JSON data and HTTP requests. Here are the key dependencies:

1. **org.json (JSON Processing Library)**: This library is used for parsing the JSON response from the API and extracting relevant data.
   - **Download link**: [org.json](https://mvnrepository.com/artifact/org.json/json)
   
2. **Apache HttpClient (for making HTTP requests)**: This library simplifies making HTTP requests to external APIs and processing responses.
   - **Download link**: [Apache HttpClient](https://mvnrepository.com/artifact/org.apache.httpcomponents/httpclient)

3. **Jackson Databind (optional)**: Can be used if you prefer using Jackson for advanced JSON handling and data binding.
   - **Download link**: [Jackson Databind](https://mvnrepository.com/artifact/com.fasterxml.jackson.core/jackson-databind)

### How We Did It

1. **Setting up the HTTP Connection**:  
   We use `HttpClient` to establish a connection to the cricket match API and retrieve the match data in JSON format. The API response includes comprehensive details such as team names, scores, and other match metadata.

2. **Parsing JSON Data**:  
   Using `org.json`, we parse the JSON response to extract key data points. This involves iterating over the array of matches and extracting relevant fields like team names and scores for each match.

3. **Computing Statistics**:
   - **Highest Score Calculation**: We loop through the matches to find the highest single innings score and store the corresponding team name.
   - **Counting High-Scoring Matches**: We iterate over the matches again, checking if the total score for both teams exceeds 300 and counting how many such matches exist.

4. **Output Results**:  
   The results of the highest score and the number of high-scoring matches are printed to the console, providing users with the requested data.

### How to Run

1. **Download and install the external JARs** mentioned above.
2. Clone this repository or download the source files.
3. Add the downloaded JAR files to your project's build path.
4. Execute the Java program to see the highest score and the count of matches with total scores above 300.

---

This project showcases how we can use Java to interact with external APIs, efficiently handle JSON data, and perform real-time computations with ease.

