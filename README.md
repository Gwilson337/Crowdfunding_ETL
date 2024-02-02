# Crowdfunding_ETL
We are using ETL format. ETL stands for Extract, Transform, and Load. This is best used when we need to combine data from multiple sources into one large repository.

In this project we are attempting build an ETL pipeline using Python, Pandas, and either using Python dictionary methods or regular expressions to extract and transform the data.

The starting resources are excel files contacts.xlsx and crowdfunding.xlsx.

We started by importing all dependencies into our jupyter notebook, which are Pandas and Numpy.

In ETL the extract stage comes first. First using the crowdfunding.xlsv... we extracted data into a Pandas DataFrame and got a brief summary of the dataframe.

We created the category and sub category of said dataframes by splitting the column into two categories.

Then list the unique category and sub category seperately.

Category and sub category ids were then made to label each one.

Next was to Export our category and subcategory as CSV files.

The 2nd part of the project was to create a campaign data frame.

We renamed columns, changed d.types and datetime formats of some columns.

Then merged the campaign, category  and sub category dataframes together.

After merging the dataframes, we cleaned it up more by removing unwanted columns and their data.

In the third part of the project we extracted data from contacts.xlsx

Created a contacts dataframe.

Renamed and re-ordered the columns.

Exported the dataframe to a csv file.

We then did the same thing using Regex instead of Pandas to create a contacts dataframe.

We changed the contact_id into an int64 datatype.

Extracted and changed the name of certain columns in the dataframe.

And Exported the dataframe into a csv file.

In the last part of our project, which is the loading part of ETL, we created a database using PgAdmin and QuickDBD.

QuickDBD was used to visualize the tables and their relationships, while PgAdmin was used to create the database.

Using QuickDBD, we created tables (catogory, subcategory, contacts and campaign) along with their data types, constraints and relationships to each other.

Switching over to PgAdmin, we created the Crowdfunding database and then imported the QuickDBD file of our tables.

We then imported each csv file into the correct corresponding tables.

After importing the table data, we ran a query of each table to see if the data was being displayed correctly.

An sql file was was then created to show the table creations and queries done in PgAdmin.
