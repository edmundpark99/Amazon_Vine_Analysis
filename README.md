# Amazon Vine Analysis: Using SQL and Google Colab

**Overview**

The purpose of this particular analysis was to analyze reviews written by members of the Amazon Vine program. Such program is intended for companies to receive reviews for their products. Because there are so many pieces of data to work with, we used Amazon Web Servuces and their Relational Database Service, to transform data and load it into a pgAdmin service and then use PySpark to assess for biases. 

The data used in question is here: https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Video_Games_v1_00.tsv.gz

**Results**

![Paid Reviews](https://user-images.githubusercontent.com/6594718/174501606-cd634e2c-8e5d-49d7-86c8-c89a5c3f1750.png)
![Unpaid Reviews](https://user-images.githubusercontent.com/6594718/174501633-d91493f2-b95e-47e9-8294-c77b343af8df.png)

- There were 94 Vine reviews concerning video games, and 40471 Non-Vine reviews

![Paid 5-Star Reviews](https://user-images.githubusercontent.com/6594718/174501666-066762b6-0d91-4b90-af17-572ec02b50c5.png)
![Unpaid 5-Star Reviews](https://user-images.githubusercontent.com/6594718/174501723-a9057e9e-090a-4508-92e1-de6693883d2b.png)

- There were 48 5-star Vine reviews concerning video games, and 15663 5-star Non-Vine reviews

![Paid 5-Star Reviews Percentage](https://user-images.githubusercontent.com/6594718/174501761-63846f4a-7987-4be5-9062-2285b1306cf1.png)
![Unpaid 5-Star Reviews Percentage](https://user-images.githubusercontent.com/6594718/174501796-e34f8236-fed2-4651-b84a-924a65aed432.png)

- 51.06% of Vine reviews for video games were 5-star reviews, and 38.70% of Non-Vine reviews for video games were 5-star reviews.

**Summary**

Individually, there is no specific positivity bias for people in the Vine program in terms of reviews for video games, as 51.06% positive reviews only indicates a slight bias towards positivity at best, relative to a 49.94% non-5-star review percentage. However, relative to unpaid, non-Vine reviews, there would be a positivity bias from Vine members, as only 38.70% of non-Vine reviews were 5-star relative to the 51.06& of Vine 5-Star reviews in this regard. One additional test we could use to further test this idea is to do an assessment of standard deviation and mean values of the review scores and amount of reviews that were 5-star, as well as other central tendency measures such as median and mode. In addition, with all of these in mind, a T-Test with paid Vine reviews versus unpaid non-Vine reviews can be conducted as well to see if there is a statistically significant difference between the two groups.
