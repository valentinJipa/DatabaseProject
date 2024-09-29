## Database Project for warehouse of contructions goods

Tools used: MySQL Workbench

Database description: The database purposes is to manage a depot of constuction material. View the quantity, orders and costs attributed with running a warehouse.

  1. Database Schema
     
     You can find below the database schema that was generated through Reverse Engineer and which contains all the tables and the relationships between them.
     
     ![Diagrama_DB](https://github.com/user-attachments/assets/e6dcb59d-5bc0-458e-9bf5-dd59d7af50ee)

     The tables are connected in the following way:
           <ul>
                <li>table lemn_masiv is connected to marfuri through a one to many relation which was implemented with lemn_masiv.id_lemn as primary key and marfuri.id_marfa_lemn as foreign key</li>
                <li>table gresie_faianta is connected to marfuri through a one to many relation which was implemented with gresie_faianta.id as primary key and marfuri.id_marfa_ceramica as foreign key</li>
                <li>table caramizi is connected to marfuri through a one to many relation which was implemented with caramizi.id as primary key and marfuri.id__marfa_caramizi as foreign key</li>
                <li>table marfuri is connected to comenzi through a one to many relation which was implemented with marfuri.id_marfa as primary key and comenzi.id_produs as foreign key</li>
                <li>table clienti is connected to comenzi through a one to many relation which was implemented with clienti.id_client as primary key and comenzi.id_client as foreign key</li>
        </ul>
  2. Database Queries
         <ul>
                <li>DDL (Data Definition Language)</li>
                The following instructions were written in the scope of CREATING the structure of the database
     
      Creating database depozit_marfa and all it's aforementioned tables:
     
      ![image](https://github.com/user-attachments/assets/2f8d3927-fb00-43e3-96a2-1a29d175db94) ![image](https://github.com/user-attachments/assets/0180ed81-32db-4fd6-b3e0-11765f988589) 
     ![image](https://github.com/user-attachments/assets/b44d550e-7afd-4f5b-aff3-c14005eb00ce) ![image](https://github.com/user-attachments/assets/d5e8534d-5257-419f-99b7-af63b1ae9747) ![image](https://github.com/user-attachments/assets/e67a82e1-fc30-4ac3-a5ce-8d95fa810769) ![image](https://github.com/user-attachments/assets/1242d47b-5235-42a2-99d8-0eec2af688e2)

     After the database and the tables have been created, a few ALTER instructions were written in order to update the structure of the database, as described below:
     
     ![image](https://github.com/user-attachments/assets/c0fde079-2101-4101-896d-cdc0e4762859) ![image](https://github.com/user-attachments/assets/b188894a-13e5-4cb4-b7ad-68761fc596f2)


     <li>DML (Data Manipulation Language)</li>
     In order to use the database I populated the tables with various data necessary in order to perform queries. In the testing process, this necessary data is identified in the Test Design phase and created in the Test Implementation phase.
     Below you can find all the insert instructions that were created in the scope of this project:
     
     ![image](https://github.com/user-attachments/assets/93025d17-cbfa-4224-b6b3-c6a4d889f0ca) ![image](https://github.com/user-attachments/assets/541beaa0-c3b1-4678-96ca-d1e98b778d87)
     ![image](https://github.com/user-attachments/assets/db803da6-6f0c-4a8f-b65a-8ca270ea557c) ![image](https://github.com/user-attachments/assets/772c2175-67e4-4848-a1d7-f0c04b5b9957)
     ![image](https://github.com/user-attachments/assets/3f6c1ebd-1de7-4995-bd13-bf0b2794fde9)

     After the insert, in order to prepare the data to be better suited for the testing process, I updated some data

     ![image](https://github.com/user-attachments/assets/66ce36af-4b4c-4932-8232-7c94b0728941)
     ![image](https://github.com/user-attachments/assets/917e67f8-1926-4b28-8854-d8167bd22bdb)

     <li>DQL (Data Query Language)</li>
     In order to simulate various scenarios that might happen in real life I created the following queries that would cover multiple potential real-life situations:
     - Here I performed 2 queries to show the name and id of all items in table 'marfuri', and show show all the items for only 1 type of pruduct
     
     ![image](https://github.com/user-attachments/assets/4fa6b6ec-ef00-48ac-a0e0-34b489417e2d)
     
     results: ![image](https://github.com/user-attachments/assets/df180cb2-137b-4fc8-8ae8-86dc3ff85cd3) ![image](https://github.com/user-attachments/assets/9df86090-efe9-46ad-b070-bbfcb6c342c9)



  </ul>



  
                  
