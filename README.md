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

# Task 1: Creating a new database and the PetRescue table

Rather than create the table manually by typing the DDL commands in the Query editor of my PgAdmin, I downloaded and executed the script containing the create table command.

The script file is available here: https://drive.google.com/file/d/1AVg-41q_HH0koUU-30hmEAYtDFEWVwUe/view?usp=sharing

![image](https://github.com/user-attachments/assets/f054243d-3a4b-4672-943b-355b721393fd)

# Task 2: Solving SQL Problems Using Aggregate Functions

1. Calculate the total cost of all animal rescues in the PETRESCUE table.

   In solving this problem, I issued the query below:

   SELECT SUM(cost) FROM petrescue;

   ![image](https://github.com/user-attachments/assets/0b6e86fe-8a4b-43da-8aa2-e84a94492cf4)

2. Display the total cost of all animal rescues in the PETRESCUE table in a column called SUM_OF_COST.

   In solving this problem, I issued the query below:

   SELECT SUM(cost) AS SUM_OF_COST
   FROM petrescue

   ![image](https://github.com/user-attachments/assets/9d230677-81d0-4a73-99ab-5dab2d30aec9)


3.  Display the maximum quantity of animals rescued.

    In solving this problem, I issued the query below:

    SELECT MAX(quantity) FROM petrescue 
   
    ![image](https://github.com/user-attachments/assets/43a8d946-944c-413b-abc2-4f0134fe173f)

4. Displays the average cost of animals rescued.

   In solving this problem, I issued the query below:
   
   SELECT AVG(cost) FROM petrescue 

   ![image](https://github.com/user-attachments/assets/9c158556-ca1a-42ec-b273-bd98afdebe2c)

    




