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

Then merge campaign dataframe and sub category dataframe together.

Then merge category and sub category dataframes together.
