# LinkedInJobRecommendation

This is a content-based job recommendation system implemented in Python. It makes job recommendations based on matching candidate skills and experience with job postings.

# Dataset
The dataset used is a sample LinkedIn job postings CSV file  from Kaggle containing columns - id, title, description, salary, location etc. The key columns used are:

title - job title
skills - list of skills required for the job
experience - level of experience required

# Approach
The recommendation system works as follows:

1. Preprocess job titles and skills to clean and lemmatize text.
2. Create TF-IDF vectors for each job based on its title + skills.
3. Create user profile vectors in a similar way based on title + skills.
4. Calculate cosine similarity between user and all job vectors to find closest matching jobs.
5. Recommend top 5 most similar jobs to the user.

Evaluation metrics like precision and recall can be calculated by splitting data into train and test sets.

# Future Work
This can be expanded to build a full-fledged job recommendation platform with UI, user accounts, and integration with job sites. Collaborative filtering approaches can also be explored.
