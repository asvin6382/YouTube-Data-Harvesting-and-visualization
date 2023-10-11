# YouTube Data Harvesting and Visualization
 - A Streamlit application that enables users to access and analyze data from multiple YouTube channels. I utilized Python, the YouTube Data API v3, MongoDB, MySQL, and Streamlit. 
## Python
- I used the Python programming language for this project because Python allows for data frames and various packages to connect to MongoDB and MySQL. Additionally, you can build a web app using Streamlit with Python
## Youtube Data API v3
- The YouTube Data API is accessed through the Google API library. Initially, you need to create an account on Google and log in to the Google Developer Console. Then, you have to enable the YouTube Data API, and from there, you can obtain a unique API key. With this API key, you can gather information about YouTube channels, videos, and even comments. Please ensure that you use the 'googleapiclient' package to connect it to Python.
## MongoDB
- I have stored the data retrieved from the YouTube API in a MongoDB data lake. MongoDB was the preferred choice for this data lake because of its ability to seamlessly handle unstructured and semi-structured data.
## MySQL 
- I used MySQL Workbench to save data from MongoDB. While working on this task, I encountered some errors, which I've outlined below for your review. It's important to note that, before data transformation, you must create a database in MySQL, define table names, and specify the respective column names. You can find the SQL code for this in the file above.
## Streamlit Web App
- I used Streamlit to create a web application. In this app, we have three tabs: 'Home,' 'Extract and Transform,' and 'View'
- In the 'Home' tab, you can access the basic features.
- The 'Extract and Transform' tab allows you to provide a YouTube channel ID and retrieve data, which you can then save in MongoDB. There's also a 'Save to SQL' button, which simplifies the process of storing data from MongoDB to MySQL.
- The 'View' tab is where you can perform in-depth analysis. I used bar charts and data frames for analytical visualizations, with the Pandas package for data frames. This area is designed for analyzing data from multiple YouTube channels
## Recounting Challenges and Solutions
- I encountered two errors during this process:
- The first error was related to the use of the Microsoft Python extension, where our file path was not saved in our environment variables as a default setting. Consequently, the Streamlit app didn't work properly. To resolve this, I uninstalled the extension and installed a new Python version from python.org. During the initial installation, I made sure to enable the 'Copy Path' checkbox, which resolved the issue.
- The second error occurred during the migration process from MongoDB to SQL data. The reason behind this error was that MongoDB can handle unstructured and complex data types, which MySQL cannot. To address this, I removed two features in videos and one feature in comments since they had list values. By using string operations, I transformed these lists of words into single strings. Although these features were removed from our analytics, they no longer posed compatibility issues.
  



## Sample Images 
### Extract and Transform Page
![Sample Image](./Screanshots/Screenshot%20(200).png)
### View Page
![Sample Image](./Screanshots/Screenshot%20(199).png)


## Project Conclusion and Thank You
-Project successfully concluded with gratitude for everyone's contributions and support. Special thanks to Vijay Kumar V, Talent Acquisition Executive at GUVI, for providing this opportunity.
