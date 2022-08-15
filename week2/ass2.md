# Week 2 Assignment 2

## Question 1

True or False: Mongo shell is a tool provided by MongoDB to interact with your databases.
>True

## Question 2

MongoDB uses compound indexing. What is special about a compound index?
>MongoDB compound indexes index more than one field.

## Question 3

Aggregation pipeline is a series of operations that you apply on your data to get a desired result. What does the following operation do?

```mongo
db.courseResults.aggregate([

{ $match: { "year": 2020 } },

{ $group: { "_id": "$courseId", "avgScore": { $avg: "$score"} } }

])
```

>Filter 2020 documents, group these documents by course, then calculate the average student score per course in that year.

## Question 4

A MongoDB Replica Set is a collection of data bearing nodes _________________
>With each node being a primary node maintaining a copy of the same data through replication. (Probably)

## Question 5

What does the following operation in Python do?

```mongo
customers.count_documents({"lastName": "Smith"})
```

>It counts the number of customers with lastname “Smith” and returns the number of records found as an outcome.
