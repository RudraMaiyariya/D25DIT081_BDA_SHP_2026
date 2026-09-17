# Practical 5: CRUD Operations, Aggregation Pipeline, and Indexing using MongoDB


## Challenges Faced


1. Understanding and executing MongoDB CRUD operations using `insertOne()`, `insertMany()`, `find()`, `updateOne()`, `updateMany()`, `deleteOne()`, `deleteMany()`, and `drop()`.
2. Writing MongoDB queries correctly using conditional operators such as `$gt`, `$lt`, `$gte`, `$lte`, `$and`, `$or`, and `$in`, along with sorting, limiting, and projection.
3. Building a multi-stage aggregation pipeline using `$match`, `$group`, `$sort`, and `$project` for branch-wise student analysis.
4. Creating an index on `student_id` and verifying query performance using `explain()` and `IXSCAN`.
5. Importing the student dataset from a JSON file using `mongoimport` and understanding that `mongoimport` must be executed from PowerShell/Windows Terminal rather than inside `mongosh`.

## Solutions


1. Created the `BDA_Practical5` database and `students` collection, then inserted student records using `insertOne()` and `insertMany()`.
2. Used MongoDB conditional, logical, sorting, limiting, and projection operators to retrieve and analyze the required student records.
3. Used `$set` with `updateOne()` and `$inc` with `updateMany()` to modify individual and multiple student documents.
4. Performed document deletion using `deleteOne()` and `deleteMany()`, and demonstrated collection removal using `drop()` on a temporary collection.
5. Implemented the aggregation pipeline with `$match`, `$group`, `$sort`, and `$project` to generate branch-wise student statistics such as total students, average marks, maximum marks, and minimum marks.
6. Created a single-field index on `student_id` and used `explain("executionStats")` to verify index-based query execution with `IXSCAN`.
7. Installed MongoDB Database Tools and used `mongoimport` from PowerShell to import the `students.json` dataset into the `students_imported` collection.
