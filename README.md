# News-Aggregator

- The News Aggregator project is a web application that collects and displays news articles from various sources in one place. It allows users to browse, filter, and search for news articles based on categories, keywords, and publication dates. The goal is to provide a centralized platform for users to access diverse news content without needing to visit multiple websites.


### Technology Used
The following technologies used to build news aggregator:

 
- **Backend:** Python, Django

- **Frontend:** HTML, CSS, Bootstrap 4, JavaScript

### Project Flow

-  User Interaction with Frontend

**Landing Page:** The user lands on the homepage, which shows the latest aggregated news articles from various sources. The homepage is designed using 
Bootstrap 4 to be responsive and visually appealing.

- Database Interaction and Processing

****Model Structure**:** Django models are used to represent the news articles, users, and any other related entities.
Relevant models include:
**Article Model:** Stores information about the fetched articles.
**Comments Model:** For user-generated content on specific articles.
**Data Management:** Admins have the ability to manually add or remove sources via Django's admin panel.

- Frontend Rendering (Homepage and Categories)

**Displaying News:** The homepage dynamically displays the aggregated news articles with the option to filter by category (e.g., politics, technology, sports).
The articles are pulled from the database and shown in a paginated manner using Django's template system.
**Search & Filters:** Users can search for articles by keywords or filter based on categories. The search query interacts with the database to find relevant articles and display the results.

- Commenting & Rating:

Users can leave comments on articles, which are displayed under each article.
They can also rate articles, with the ratings being aggregated and displayed.

-  Admin Functionality

**Admin Dashboard**: Admins can log into the Django admin panel to ### manage articles, users, and comments.
This includes:
Approving or deleting news sources.
Modifying or removing articles.
Managing user accounts, banning users if needed.
**Content Moderation:**
Admins can monitor and delete inappropriate comments or content.

### Summary

The News Aggregator is a web-based application designed to collect and display news articles from multiple sources in one unified platform. Developed using Python and Django, this project automates the process of gathering news through APIs or web scraping, enabling users to access a wide variety of news articles in one place. The project focuses on improving the user's reading experience by providing search, filtering, bookmarking, and personalized recommendations.



## Models
----------------
-   Category
    -   Title
    -   Image
-   News
    -   Category
    -   Title
    -   Image
    -   Detail
-   Comments
    -   News
    -   Name
    -   Email
    -   Comments
    -   Status

## Templates
---------------------
-   views.py
-   urls.py
-   project/urls.py
-   templates
    -   base.html
    -   index.html
    -   category.html
    -   detail.html
