## Database Project for warehouse of contructions goods

Tools used: MySQL Workbench

Database description: The database purposes is to manage a depot of constuction material. View the quantity, orders and costs attributed with running a warehouse.

  1. Database Schema
     
     You can find below the database schema that was generated through Reverse Engineer and which contains all the tables and the relationships between them.
     
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
        </ul>

     The following instructions were written in the scope of CREATING the structure of the database
