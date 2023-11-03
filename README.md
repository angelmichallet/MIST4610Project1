# Team 3 MIST 4610 Group Project 1

## Team Name

39217 Group 3	
## Team Members
Include information about the name of the team based on the team name assigned to the team on
ELC. Also include the names of all team members as well as links to their corresponding github
repos that have the project on them.
1. 
2. 
3. 
4.  
5. 
6. 
## Project Description

This project involves the development of a relational database to streamline and manage the operations of Tennis Haven Club, a tennis facility based in Athens, Georgia. At the heart of the model is the Member entity, representing the diverse clientele we serve, from beginners to seasoned players. The club's facilities include various types of tennis courts (outdoor, indoor, clay), a pro shop, and an array of coaching options, all integral to our service offerings. These elements form key entities in our database, such as Court Bookings, Tournaments, Coaching Sessions, and Pro Shop Sales. Our aim is to accurately map the relationships between these entities, ensuring a comprehensive understanding of the club’s operations. Additionally, we're focused on creating realistic sample data to populate these entities, which will enable us to execute meaningful queries. These queries are intended to yield insights into member engagement, facility utilization, sales performance, and overall operational efficiency, guiding strategic decisions for the club's growth and success.

## Data Model

Include a screenshot of the data model. An explanation of the data model including the
relationships between the entities in natural English. Please include any screenshots of any of
the substantive conversations you have had with your client that have informed the data model.
## Data Dictionary
The data dictionary explains the different columns in the different tables including data types and
their roles. Please refer to sample present on ELC.
## Queries
Include a natural language description of the query and a justification as to why each query is
relevant from a managerial perspective (why would a manager be interested in the query results).
Avoid having queries that are almost identical to one another. You may include screenshots of the
query as well as the response of each query. You can also use the code markdown to highlight the
SQL code and copy and paste the results into the file.
To ensure the complexity of the queries some of the things that may be considered include
multiple table join, subquery, correlated subquery, GROUP BY, GROUP BY with HAVING,
multi condition WHERE, Built-in functions (e.g., AVG) or a calculated field, REGEXP, NOT
EXISTS, and more.

You may combine some of the preceding list of features into a single query (still have to provide
10 queries). Indicate in matrix format in your report which features are covered in a query. A
sample matrix is shown in the project guidelines

### Query 1
Query 1 is designed to identify all members who have registered to participate in a specific tournament, identified by the tournament ID 'tourney1'. It extracts a list that includes each participating member's unique ID, first name, and last name, alongside the tournament ID they are associated with. From a managerial perspective, this query is relevant because it helps the club's management to quickly ascertain who is taking part in one of their key events, the tournament with ID 'tourney1'. This information is crucial for organizing the event, including scheduling matches, preparing facilities, and communicating with participants. It also aids in gauging the popularity of the event and assists in future planning for similar events by providing insights into participant engagement.

DELIMITER $$
CREATE PROCEDURE TP_Q1()
BEGIN
    SELECT Member.memberID, Member.memberFirstName, Member.memberLastName, Participant.tournamentID
    FROM Participant
    JOIN Member ON Participant.memberID = Member.memberID
    WHERE Participant.tournamentID = 'tourney1';
END$$
DELIMITER ;

CALL TP_Q1;

<img width="800" alt="image" src="https://github.com/angelmichallet/MIST4610Project1/assets/130924513/bfaeb96b-d6ad-4755-a084-7dfa28036cf0">

## Database Information
The name of the database on the MySQL server. Each table should be populated with enough
data so that the queries return a sufficient result set. All queries should be bookmarked through
the use of stored procedures (take a look at the example under Module 7) according to this
format: TP_Qx (where x is to be replaced by the query number).
