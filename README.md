# spark-movielens-analytics
Scalable, distributed data processing and analytics on the MovieLens dataset using Apache Spark to study user engagement, content popularity, and interaction patterns at scale.

# Spark MovieLens Analytics

Scalable, distributed data processing and analytics on the MovieLens dataset using Apache Spark to study user engagement, content popularity, and interaction patterns at scale.

---

## 📊 Dataset
This project uses the MovieLens dataset, which contains:
- **movies.csv** — movie metadata and genre information
- **ratings.csv** — user ratings for movies
- **tags.csv** — user-generated tags associated with movies

---

## 🧠 Project Objective
The objective of this project is to design **correct and scalable analytical pipelines** using Apache Spark (PySpark), focusing on data modeling, aggregation correctness, and ranking logic in a distributed environment.

---

## 🔍 Analytical Questions Addressed
- Aggregated number of ratings per year
- Average monthly number of ratings
- Rating level distribution
- Movies that are tagged but not rated
- Movies that are rated but not tagged
- Rated but untagged movies with more than 30 user ratings
- Average number of tags per user and per movie
- Users who tagged movies without rating them
- Average number of ratings per user and per movie
- Predominant (frequency-based) genre per rating level
- Predominant tag per genre and most tagged genres
- Most predominant (popularity-based) movies
- Top movies based on average rating (with minimum user threshold)

---

## ⚙️ Technologies Used
- Apache Spark (PySpark)
- Databricks
- Distributed storage (DBFS)
- Spark DataFrame API
- Window functions (`dense_rank`)
- Aggregations and joins


---

## 📝 Implementation Notes
- The project is implemented entirely using the PySpark DataFrame API.
- Data was processed on distributed storage using Databricks.
- Window functions were used to compute ranking-based insights while handling ties deterministically.
- Explicit join semantics were applied to ensure analytical correctness.

---

## 🚀 Key Takeaway
In large-scale data systems, **correct data modeling and join semantics are more important than individual transformations**.  
This project highlights how careful handling of data grain and aggregation logic is critical for producing reliable analytical results.
