# Data Management CQL and SQL
## Introduction
Use Cassandra Query Language (CQL) and Spark2 Structured Query Language (SQL)
The data used in this project is available for download in data.zip, using u.data, u.item and u.user.

u.data     -- The full u data set, 100000 ratings by 943 users on 1682 items.
              Each user has rated at least 20 movies.  Users and items are
              numbered consecutively from 1.  The data is randomly
              ordered. This is a tab separated list of 
	         user id | item id | rating | timestamp. 
              The time stamps are unix seconds since 1/1/1970 UTC   

u.item     -- Information about the items (movies); this is a tab separated
              list of
              movie id | movie title | release date | video release date |
              IMDb URL | unknown | Action | Adventure | Animation |
              Children's | Comedy | Crime | Documentary | Drama | Fantasy |
              Film-Noir | Horror | Musical | Mystery | Romance | Sci-Fi |
              Thriller | War | Western |
              The last 19 fields are the genres, a 1 indicates the movie
              is of that genre, a 0 indicates it is not; movies can be in
              several genres at once.
              The movie ids are the ones used in the u.data data set.

u.user     -- Demographic information about the users; this is a tab
              separated list of
              user id | age | gender | occupation | zip code
              The user ids are the ones used in the u.data data set.

## Output result
i) Calculate the average rating for each movie.

![WhatsApp 图像2024-06-21于11 16 39_0d1d0c52](https://github.com/PanLuochuan/Data-Management-CQL-and-SQL/assets/152348928/885bcf06-d61c-4197-b5b3-956437fda762)

ii) Identify the top ten movies with the highest average ratings.

![WhatsApp 图像2024-06-21于11 16 39_142bb843](https://github.com/PanLuochuan/Data-Management-CQL-and-SQL/assets/152348928/1bbd437f-e9f1-4340-8134-8121fe2dff5b)

iii) Find the users who have rated at least 50 movies and identify their favourite movie genres.

![WhatsApp 图像2024-06-21于11 16 38_2c4299b3](https://github.com/PanLuochuan/Data-Management-CQL-and-SQL/assets/152348928/0122e1bb-8dd6-4327-9c4d-48292ad1d1b2)
![WhatsApp 图像2024-06-21于11 16 38_14e602b3](https://github.com/PanLuochuan/Data-Management-CQL-and-SQL/assets/152348928/735acb0a-c777-4245-a57c-d349b0feb95d)


iv) Find all the users with age that is less than 20 years old.

![WhatsApp 图像2024-06-21于11 16 39_2e26cc65](https://github.com/PanLuochuan/Data-Management-CQL-and-SQL/assets/152348928/9cbd5bd5-87e0-4dde-aa63-a638a24bbd42)

v) Find all the users who have the occupation “scientist” and their age is between 30 and 40 years old.

![WhatsApp 图像2024-06-21于11 16 55_4dd612f9](https://github.com/PanLuochuan/Data-Management-CQL-and-SQL/assets/152348928/5e106162-6666-43c0-bbed-2e64a6959001)
