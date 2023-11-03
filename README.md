# Team 3 MIST 4610 Group Project 1

## Team Name

39217 Group 3	
## Team Members
Include information about the name of the team based on the team name assigned to the team on
ELC. Also include the names of all team members as well as links to their corresponding github
repos that have the project on them.
1. Angel Michallet [@angelmichallet](https://github.com/angelmichallet)
2. Akhilesh Eloore [@akhileshe](https://github.com/akhileshe)
3. Rishi Patel [@rp65029](https://github.com/rp65029)
4. Daniel Zavala-palafox [@dzavalapalafox](https://github.com/dzavalapalafox)
5. Penn Worden [@pennworden](https://github.com/pennworden)
6. Noah Martin [@noahhmartin03](https://github.com/noahhmartin03)
   
## Project Description

This project involves the development of a relational database to streamline and manage the operations of a tennis facility based in Athens, Georgia. At the heart of the model is the Member entity, representing the diverse clientele we serve, from beginners to seasoned players. The club's facilities include various types of tennis courts (outdoor, indoor, clay), a pro shop, and an array of coaching options, all integral to our service offerings. These elements form key entities in our database, such as Court Bookings, Tournaments, Coaching Sessions, and Sales. Our aim is to accurately map the relationships between these entities, ensuring a comprehensive understanding of the club’s operations. Additionally, we're focused on creating realistic sample data to populate these entities, which will enable us to execute meaningful queries. These queries are intended to yield insights into member engagement, facility utilization, sales performance, and overall operational efficiency, guiding strategic decisions for the club's growth and success.

## Data Model
Our tennis data model is intricately designed with the Member entity at its core, encapsulating the club's focus on its members and their engagement with various facilities and activities. This central role of the Member entity is underlined by several one-to-many relationships, as well as associative entities that connect Members to other critical aspects of the club's operations.

Member interaction begins with the Booking associative entity, which details their Court reservations, linking each Member to their reserved times and courts in a one-to-many fashion. This ensures that our members have access to the facilities at their preferred times while allowing us to efficiently manage and allocate court space.

These Members also partake in Tournaments, where their participation is documented through the Participant associative entity. This one-to-many relationship allows us to track which member is participating in which tournament, managing the competitive spirit of the club effectively.

Beyond the courts, Members contribute to the club's economy through Sales. Each Sale they make is connected to the Pro Shop Items they purchase, a relationship detailed by the Sale Details associative entity. These links are essential for inventory control and provide insights into purchasing trends and member preferences.

The ongoing upkeep of the Courts is vital to providing a top-tier playing experience. Each Court has a maintenance history, chronicled in the Maintenance Log, a one-to-many relationship that enables us to keep a close eye on the condition and availability of the facilities for members.

Members' development in the sport is fostered through Coaching Sessions, where their attendance is marked by the Attendee associative entity. This one-to-many relationship highlights our commitment to personalized training and skill improvement, with each Member attending multiple sessions tailored to their development needs.

Events are the social fabric that weaves the members together, and their participation in these events is tracked by the Event Participant associative entity between Event and Member. This relationship showcases the club's vibrant community life, with members engaging in a variety of events from social mixers to skill workshops. Each event is also thoughtfully planned and executed by multiple Staff members to provide the best member experience. Staff at the club are integral to the seamless operation of the facilities and services. They are also the custodians of the courts, ensuring that each court is adequately prepared and maintained, reflected in the one-to-many relationship between Staff and Court. Additionally, within the Staff members are those with coaching roles, illustrated in the one-to-many relationship of a staff member being able to teach a range of Coaching Sessions.

<img width="821" alt="image" src="https://github.com/angelmichallet/MIST4610Project1/assets/130924513/5489e4ce-1804-4c88-9ac3-7143ea11d140">

To avoid unecessary clutter of screenshots, below is a link to our chat with our client (ChatGPT) to start the base of our data model. We required making additional appropriate changes and edits to the information provided by out client to clarify our entities, relationships, and attributes

[Client Conversation](https://chat.openai.com/share/57c8fb61-4bba-411b-98e5-283420a0bc06)

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
<img width="1211" alt="image" src="https://github.com/angelmichallet/MIST4610Project1/assets/130924513/d9497122-1942-4e9f-8344-4e343c7c1b89">

### Query 2


### Query 3


### Query 4


### Query 5


### Query 6


### Query 7


### Query 8


### Query 9


### Query 10




## Database Information
Name of database: ns_F2339217Group3

Additional information: Each query listed above is marked in the database using stored procedures which can be called using the following format: CALL TP_Qx(), where x is to be replaced by the query number


