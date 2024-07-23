# Hands-on Exercises on Built-in functions - Aggregate, Scalar, String, Date and Time Functions in PostgreSQL

In this hands-on exercises, I demonstrated skills in writing SQL statements using Built-in functions - Aggregate, Scalar, String, Date and Time Functions in PostgreSQL

# Software Used in this Lab

PgAdmin 4 (PostgreSQL 15)

# Database Used in this Lab

The dataset used in this hands-on exercises is called PETRESCUE and is gotten from IBM. 

PETRESCUE TABLE

![image](https://github.com/user-attachments/assets/dc1c3b93-d317-4087-b9ec-df797d22e60c)

# Objectives

The objectives of the hands-on excercises are to:

1. Compose and run sub-queries with multiple tables
2. Check query results and view log files

# Task A: Creating a new database and the PetRescue table

Rather than create the table manually by typing the DDL commands in the Query editor of my PgAdmin, I downloaded and executed the script containing the create table command.

The script file is available here: https://drive.google.com/file/d/1AVg-41q_HH0koUU-30hmEAYtDFEWVwUe/view?usp=sharing

![image](https://github.com/user-attachments/assets/f054243d-3a4b-4672-943b-355b721393fd)

# Task B: Solving SQL Problems Using Aggregate Functions

1. Calculate the total cost of all animal rescues in the PETRESCUE table.

   In solving this problem, I issued the query below:

   SELECT SUM(cost) FROM petrescue;

   ![image](https://github.com/user-attachments/assets/0b6e86fe-8a4b-43da-8aa2-e84a94492cf4)

2. Display the total cost of all animal rescues in the PETRESCUE table in a column called SUM_OF_COST.

   In solving this problem, I issued the query below:

   SELECT SUM(cost) AS SUM_OF_COST
   FROM petrescue;

   ![image](https://github.com/user-attachments/assets/9a18bab2-f583-428d-aee7-c63c5dcdd74c)


3.  Display the maximum quantity of animals rescued.

    In solving this problem, I issued the query below:

    SELECT MAX(quantity) FROM petrescue;

    ![image](https://github.com/user-attachments/assets/4ba5b6f7-270c-4d99-ac29-160b775eda06)


5. Displays the average cost of animals rescued.

   In solving this problem, I issued the query below:

   SELECT AVG(cost) FROM petrescue

   ![image](https://github.com/user-attachments/assets/dd99506c-b206-48f0-a7d0-dde1516cef5d)

7. Display the average cost of rescuing a dog.

   In solving this problem, I issued the query below:

   SELECT AVG(cost/quantity)
   FROM petrescue
   WHERE animal = "Dog";

   ![image](https://github.com/user-attachments/assets/acdff2c8-b347-4b6a-943e-2c03f4268745)

# Task C: Solving SQL Problems Using Scalar and String Functions

1. Display the rounded cost of each rescue.
 
   In solving this problem, I issued the query below:

   SELECT ROUND(cost) FROM petrescue;

   ![image](https://github.com/user-attachments/assets/020a15e6-da53-434a-a952-0a10ec5f10bd)

2. Display the length of each animal name.

    In solving this problem, I issued the query below:

    SELECT LENGTH(animal) FROM petrescue;

    ![image](https://github.com/user-attachments/assets/61061a63-c6f7-45ef-a662-102ccc1b64bc)

3. Display the animal name in each rescue in uppercase.

   In solving this problem, I issued the query below:

   SELECT UPPER(animal) FROM petrescue;

   ![image](https://github.com/user-attachments/assets/5bed4df4-2e4c-49e5-beab-77f16a3acd25)

4. Display the animal name in each rescue in uppercase without duplications.

   In solving this problem, I issued the query below:

   SELECT UPPER(DISTINCT animal) FROM petrescue;
    
   ![image](https://github.com/user-attachments/assets/abe4847c-e424-4a2f-a1ca-d375a88cfda1)

5. Display all the columns from the PETRESCUE table, where the animal(s) rescued are cats. Use cat in lower case in the query.
    
   In solving this problem, I issued the query below:

   SELECT * FROM petrescue
   WHERE ;
    

17. Display the day of the month when cats have been rescued.

    In solving this problem, I issued the query below:

18. Displays the number of rescues on the 5th month.

    In solving this problem, I issued the query below:

19. Displays the number of rescues on the 14th day of the month.
    
    In solving this problem, I issued the query below:

20. Animals rescued should see the vet within three days of arrivals. Enter a function that displays the third day from each rescue.

    In solving this problem, I issued the query below:

21. Displays the length of time the animals have been rescued; the difference between today’s date and the rescue date.

    In solving this problem, I issued the query below:


   

   


