<Overview>

This project contains SQLPlus scripts for managing and analyzing data in a Zoo Management System. It includes the database schema, sample data for tables, and SQL reports to extract meaningful insights from the data. The project is designed to be run in Oracle SQL*Plus or any compatible SQL environment.
The database captures details about:

Visitors
Restaurants and restaurant orders
Shops and purchases
Animal shows and show participation
Tram rides and ticketing
Maintenance tasks and enclosures
Database Structure
The database includes tables such as:
visitor – visitor details
restaurant & restaurant_order – restaurants and orders
shop, shop_item, purchase, purchase_item – shop and purchase management
animal & animal_show & animal_show_participation & animal_show_attendance – animal shows
tram & tram_ride & tram_ride_ticket & tr_ticket_type – tram rides and ticketing
ticket_type_3nf & entry_ticket_3nf – ticketing system
enclosure & maintenance – zoo enclosures and maintenance tasks

All tables include primary and foreign keys where applicable, and constraints such as uniqueness on identifiers.

<Reports>

The project contains SQL scripts to generate 3 interactive reports. The reports included are:

Ticket Type Sales Report – Shows the total tickets sold for selected ticket types, with a grand total of tickets sold.
Maintenance Status Count in Enclosures – Counts maintenance activities in enclosures based on selected status, showing total tasks per enclosure.
Total Revenue by Ticket Type – Calculates revenue for a selected ticket type, showing total tickets sold and total revenue generated.

<Usage>

Ensure all database tables exist and are populated with sample or real data.
Open Oracle SQL*Plus (or compatible SQL client).
Run the SQL scripts using:
@path_to_your_sql_file.sql
Follow interactive prompts for inputs such as zones, ticket types, dates, or shop/item names.
Review the output directly in the SQL client.

<Notes>
Scripts assume the user has sufficient permissions to query all tables.
Interactive prompts (ACCEPT) are used in reports for dynamic filtering.

All reports include computed totals and formatted output for readability.
