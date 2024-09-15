## Database Project for warehouse of contructions goods

Tools used: MySQL Workbench

Database description: The database purposes is to manage a depot of constuction material. View the quantity, orders and costs attributed with running a warehouse.

  1. Database Schema
     
     You can find below the database schema that was generated through Reverse Engineer and which contains all the tables and the relationships between them.
     
     The tables are connected in the following way:
           <ul>
                <li>table lemn_masiv is connected to marfuri through a one to many relation which was implemented through the primary key lemn_masiv.id_lemn as primary key and marfuri.id_marfa_lemn as foreign key</li>
           </ul>
