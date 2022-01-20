# MTSU HackMT 2022

## Overview

This is a public repository for the Data Science Club team to use for collaboration for the MTSU HackMT 2022.  Please check out the recommended resources and tools in preparation for the event.  We will be using a combination of Anaconda and Google Colab.  Anaconda is a tool that manages installing Python and Python packages.  Google Colab is a free online platform for running jupyter notebooks.

## Background and Problem Statement

In the United States, there are over 1.5 million non-profit organizations, ranging in services from homeless shelters to professional organizations. Though they all offer much needed services, most of them are difficult to locate and go largely unnoticed by those who need them. Additionally, very few of them work together to offer a suite of services, that if offered, would provide a person with the support, skills training, and connections necessary to help them. [Project Maslow](https://www.projectmaslow.org/) is connecting the non-profit network and making their services available for anyone who seeks assistance or growth. And by connecting non-profit services thoughtfully, we are using data analytics and AI, we will be able to help individuals plot a path to anywhere they wish to go. Our mission is to connect people, resources, and community to create endless opportunity.

For the Hackathon challenge, since non-profit organizations operate using mission statements and they don’t have the published service categories that are needed, you will be helping determine what services are offered using tax data from the IRS for all non-profits that have applied for non-profit status in the US over the last 7 years. The data set is large and in free-form text, describing multiple non-profit businesses. Since Project Maslow will require knowing what services are offered by the non-profits in the non-profit network, you will use natural language processing and any other tools at your disposal to categorize these great organizations using their descriptions and you will plot them geographically based on their locations. Project Maslow will use your results to launch their first functioning prototype.

## Data Files

The [project_maslow_starter_notebook](project_maslow_starter_notebook.ipynb) includes python code that will take care of downloading the Project Maslow files and has functions that takes care of loading the files into dataframes.

### nonprofit.txt

This file contains information about the non-profit such as the non-profit's name, address, phone number, ein, and reporting year.  This will be useful in creating mapping visualizations highlight where different types of non-profits are geographically located

|column_name|data_type|
|-|-|
|nonprofit_id|Int64|
|reporting_year|Int64|
|ein|Int64|,
|businessname|str|
|phone|str|
|address1|str|
|address2|str|
|city|str|
|stabbrv|str|
|zip|str|

### nonprofit_text.txt

This file contains descriptions of the non-profits in the `description` column that will be used for mining what kind of service the non-profit offers.  There is a `nonprofit_id` that can be used to join this back a non-profits information for data visualization.

|column_name|data_type|
|-|-|
|nonprofit_text_id|Int64|
|reporting_year|Int64|
|nonprofit_id|Int64|
|grouptype|str|
|description|str|

## Recommended Resources

|Resource|Link|
|-|-|
|Data Science Club Shared Drive|https://drive.google.com/drive/folders/1IVXOzzSaIVGTgsOKX2mJULvXHsbm-DJ9|
|HackMT 2022 Registration|https://www.eventbrite.com/e/hackmt-2022-tickets-208620608857|

## Recommended Tools

Please check out the following tools prior to the event and if possible, have Anaconda installed.  Google Colab is an alternative to Anaconda for running Jupyter Notebooks in the cloud. Google Colab requires a Google Account.

|Tool|Description|Link|
|-|-|-|
|Jupyter Notebook/Lab|Jupyter notebooks are a popular way for Data Scientists/Analysts to analyze/model data with Python|https://jupyter.org/|
|Anaconda|Tool for managing python versions and packages|https://www.anaconda.com/products/individual|
|Google Colab|Google Colab is a free online platform to running jupyter notebooks|https://colab.research.google.com/|