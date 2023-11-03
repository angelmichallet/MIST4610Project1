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

To avoid unecessary clutter of screenshots, below is a link to our chat with our client (ChatGPT) to start the base of our data model. We required making additional appropriate changes and edits to the information provided by our client to clarify our entities, relationships, and attributes.

[Client Conversation](https://chat.openai.com/share/57c8fb61-4bba-411b-98e5-283420a0bc06)

## Data Dictionary
<img width="715" alt="Screenshot 2023-11-03 at 6 52 49 PM" src="https://github.com/angelmichallet/MIST4610Project1/assets/132240342/ea793005-2646-4ea7-b841-74987cf94028">

<img width="722" alt="Screenshot 2023-11-03 at 6 54 36 PM" src="https://github.com/angelmichallet/MIST4610Project1/assets/132240342/022e526a-684b-4740-b68d-025203da5add">

<img width="722" alt="Screenshot 2023-11-03 at 6 54 56 PM" src="https://github.com/angelmichallet/MIST4610Project1/assets/132240342/20542c25-01f8-4ab7-bcc7-828c62f56886">

<img width="720" alt="Screenshot 2023-11-03 at 6 55 18 PM" src="https://github.com/angelmichallet/MIST4610Project1/assets/132240342/64dc4920-bc18-43ec-87ab-7a1046325c9a">

<img width="716" alt="Screenshot 2023-11-03 at 6 55 44 PM" src="https://github.com/angelmichallet/MIST4610Project1/assets/132240342/a5b20677-8bfa-414e-aea8-9c07ba963c6c">

<img width="705" alt="Screenshot 2023-11-03 at 6 57 18 PM" src="https://github.com/angelmichallet/MIST4610Project1/assets/132240342/484ac990-dd9f-4965-a12f-53cdfd9d5837">

<img width="710" alt="Screenshot 2023-11-03 at 6 57 56 PM" src="https://github.com/angelmichallet/MIST4610Project1/assets/132240342/7ea7aef6-e333-4106-b441-53aba4ec11e2">

<img width="719" alt="Screenshot 2023-11-03 at 6 58 47 PM" src="https://github.com/angelmichallet/MIST4610Project1/assets/132240342/65b8bbda-4a23-4e24-a679-8b10598ca2c6">

<img width="706" alt="Screenshot 2023-11-03 at 6 59 31 PM" src="https://github.com/angelmichallet/MIST4610Project1/assets/132240342/088bc311-1fc8-4c1f-81ae-6d86022fe96a">

<img width="717" alt="Screenshot 2023-11-03 at 6 59 52 PM" src="https://github.com/angelmichallet/MIST4610Project1/assets/132240342/a4b219a4-a09e-4801-8072-fdb65fa6f1cf">

<img width="699" alt="Screenshot 2023-11-03 at 7 00 26 PM" src="https://github.com/angelmichallet/MIST4610Project1/assets/132240342/b5dd92ad-e4ef-43b3-a728-50b20fe5d5e3">

<img width="700" alt="Screenshot 2023-11-03 at 7 00 54 PM" src="https://github.com/angelmichallet/MIST4610Project1/assets/132240342/ce9c176f-8d47-4383-81a8-4199dd4c3566">

<img width="708" alt="Screenshot 2023-11-03 at 7 01 24 PM" src="https://github.com/angelmichallet/MIST4610Project1/assets/132240342/e53d3b21-6839-436e-8630-ac3aa9078b6b">

<img width="707" alt="Screenshot 2023-11-03 at 7 01 55 PM" src="https://github.com/angelmichallet/MIST4610Project1/assets/132240342/4b78868f-7899-48b8-a863-74dc8c14e718">


## Queries
### Matrix Table
<img width="662" alt="image" src="https://github.com/angelmichallet/MIST4610Project1/assets/130924513/2e624506-0771-446a-a018-94a9d6ca5e0e">

### Query 1
Query 1 is designed to identify all members who have registered to participate in a specific tournament, identified by the tournament ID 'tourney1'. It extracts a list that includes each participating member's unique ID, first name, and last name, alongside the tournament ID they are associated with. From a managerial perspective, this query is relevant because it helps the club's management to quickly ascertain who is taking part in one of their key events, the tournament with ID 'tourney1'. This information is crucial for organizing the event, including scheduling matches, preparing facilities, and communicating with participants. It also aids in gauging the popularity of the event and assists in future planning for similar events by providing insights into participant engagement.

<img width="1198" alt="image" src="https://github.com/angelmichallet/MIST4610Project1/assets/130924513/828c3dfc-9c5e-40ee-9284-a5df2674fc77">

### Query 2
Query 2 is designed to calculate and rank the profitability of items sold in the Pro Shop. It determines the individual return on investment (ROI) for each item by comparing the selling price to the purchase cost and expressing this as a percentage. It also calculates the total profit made from each item by considering the quantity sold. The results are then ordered to show the most profitable items at the top. A manager may find this data useful as it highlights which items contribute most to the Pro Shop's earnings and helps in making informed decisions about inventory management, pricing strategies, and which items to promote or potentially discontinue based on their profitability. 

<img width="1206" alt="image" src="https://github.com/angelmichallet/MIST4610Project1/assets/130924513/7df2769b-1147-486e-892b-30a65090f3e9"> 

### Query 3 
Query 3 retrieves a list of first and last names of members who have attended coaching sessions that were conducted by a staff member named Una Ridler. It does this by first finding all session IDs associated with Una Ridler, and then matching those sessions with the attendees of those sessions to find the corresponding members. For a manager, this information is valuable as it provides insights into the clientele of a specific coach. As Una Ridler is a coach at the tennis club, understanding her reach and impact on the members can help assess her performance and popularity. It could also be used to schedule her sessions effectively, plan for future hiring based on the demand for her coaching, or offer targeted promotions to the members who attend her sessions. This level of detail helps the manager make informed decisions about staff scheduling, member engagement, and overall operational efficiency. 

<img width="1199" alt="image" src="https://github.com/angelmichallet/MIST4610Project1/assets/130924513/d59f3be9-3999-4ec5-bea9-803f26f71fab">

### Query 4
Query 4 identifies members of the tennis club who have not made any court bookings and have not purchased any tennis rackets from the pro shop, with the additional condition that their membership began before November 3, 2022. A manager may find be interested in this information because it helps to identify members who may not be fully engaged with the club's facilities and services. Understanding who these members are allows the management to target them with specific promotions or outreach efforts to increase their engagement and potentially generate more sales or bookings, ultimately aiming to enhance their club experience and retain their membership.

<img width="1202" alt="image" src="https://github.com/angelmichallet/MIST4610Project1/assets/130924513/d22c5b64-e47c-48b0-b9cd-18215cdf6f49">

### Query 5
Query 5 is designed to identify events at the tennis club that have a higher number of participants than the average across all events. It lists each event by its ID and name, along with the count of participants for that event. The query then filters out any events where the participant count is not greater than the average participant count for all events. This information can be important to a manager to highlight which events are particularly successful in terms of attendance, potentially indicating their popularity or the effectiveness of their promotion. Understanding which events draw larger crowds can guide decisions on resource allocation, scheduling, and planning for future events to maximize engagement and profitability for the club. It can also help in identifying the types of events that resonate with the club's members, informing more strategic event planning and marketing efforts.

<img width="1200" alt="image" src="https://github.com/angelmichallet/MIST4610Project1/assets/130924513/0ca3e174-ce3f-4b2f-8a84-c26f17bf803a">

### Query 6
Query 6 summarizes and lists the total amount of money each member has spent on coaching sessions at the tennis club. It specifically focuses on members who have spent more than $20 in total. The results are organized by each member's first and last name and show a total of the fees paid for all the coaching sessions they've attended. The results are ordered from the highest spender to the lowest. This information is crucial to a manager for identifying the most engaged members, understanding revenue distribution from coaching sessions, and potentially recognizing members who might be candidates for loyalty programs or targeted promotions. It can also indicate the success of the coaching program and help in making decisions about resource allocation, pricing strategies, and planning additional services or offers.

<img width="1210" alt="image" src="https://github.com/angelmichallet/MIST4610Project1/assets/130924513/cce1a183-95b0-4936-b99b-d392b285d1d6">

### Query 7
Query 7 generates a list of unique members who joined the tennis club in the years 2020 or 2021 and have participated in one or more tournaments but have not made any purchases at the Pro Shop. For each member, it provides their ID, name, contact number, and the date they joined the club, as well as the total number of tournaments they have competed in. A manager can use this data because it identifies active and potentially loyal club members who are not engaging with one of the club's revenue streams, the Pro Shop. Understanding this can help the manager to investigate why these members have not made purchases—whether it's due to a lack of interest, awareness, or appeal of the products offered—and to develop targeted strategies to convert these active members into customers, thereby potentially increasing the club's sales and revenue.

<img width="1214" alt="image" src="https://github.com/angelmichallet/MIST4610Project1/assets/130924513/27491cd9-b30b-4996-a795-26525b0ce000">

### Query 8
Query 8 identifies members of the tennis club who have spent more than the average amount in their respective membership categories at the Pro Shop. It lists out these members by their first and last names, along with the sum of their expenditures. The purpose of the query is to highlight those members who are high spenders compared to others with the same type of membership. This information would be valuable for recognizing and possibly rewarding members who contribute significantly to the club's revenue through their purchases. Additionally, this could inform the club's marketing strategies, such as offering targeted promotions to encourage continued or increased spending among these key customers.

<img width="1210" alt="image" src="https://github.com/angelmichallet/MIST4610Project1/assets/130924513/34c2bd8a-d4a8-4b54-940f-e2670ec0271f">

### Query 9
Query 9 displays all the tournament winners’ names, the tournament they won, and the portion of the prize money they took home. Tournaments have multiple events, therefore any player who won 6 games is a winner of that tournament. The total prize money of the tournament is then split equally amongst the winners. To a manager, this information could be crucial for analyzing the outcomes of tournaments, particularly understanding how prize money is distributed among top-performing participants. It may help in financial planning, assessing the competitiveness of tournaments, and potentially in making decisions about future prize distributions or structuring of tournament brackets. This data could also be used in reporting to stakeholders about the outcomes of events and for promotional or motivational purposes within the club.

<img width="1205" alt="image" src="https://github.com/angelmichallet/MIST4610Project1/assets/130924513/50e2f9fb-9db4-4b9e-abdf-fdef28d0b7f7">

### Query 10
Query 10 retrieves a list of members who have either 'Platinum' or 'Gold' membership status, along with the dates they have made court bookings. It specifically filters out those members who have attended any coaching sessions, thus focusing only on those who are utilizing court bookings but not coaching services. The list is sorted by the members' last names. This data holds value to a manager because it identifies high-tier members (who typically contribute more to the club's revenue) that are not participating in coaching sessions. Understanding this pattern could help in tailoring specific marketing strategies or outreach programs to encourage these members to take advantage of the coaching services offered by the club. It's a way to increase engagement and potentially generate more revenue from existing high-value customers.

<img width="1201" alt="image" src="https://github.com/angelmichallet/MIST4610Project1/assets/130924513/1b97dbbf-2e7b-4442-b7eb-7bdf41d60835">

## Database Information
Name of database: ns_F2339217Group3

Additional information: Each query listed above is marked in the database using stored procedures which can be called using the following format: CALL TP_Qx(), where x is to be replaced by the query number


