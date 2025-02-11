# SQL-Project
## 1. Select all from cleaned_file
```sql
SELECT * FROM cleaned_file;
```
<img width="1124" alt="Screenshot 1446-08-12 at 11 44 01 AM" src="https://github.com/user-attachments/assets/76b48d72-b769-4293-a453-a6dd13e4f923" />

## 2. Count total records
```sql
SELECT COUNT(*) FROM cleaned_file;
```
<img width="172" alt="Screenshot 1446-08-12 at 11 45 31 AM" src="https://github.com/user-attachments/assets/9aee21ea-7392-4a66-b4f9-e628c041c2c7" />

## 3. Retrieve all unique genres
```sql
SELECT DISTINCT genre FROM cleaned_file;
```
<img width="182" alt="Screenshot 1446-08-12 at 11 47 33 AM" src="https://github.com/user-attachments/assets/113c46db-4a97-4f3a-9f1b-d09ba24bf3bc" />

## 4. Find the top 5 highest-rated places
```sql
SELECT name, rating FROM cleaned_file ORDER BY rating DESC LIMIT 5;
```
<img width="191" alt="Screenshot 1446-08-12 at 11 49 45 AM" src="https://github.com/user-attachments/assets/2464ce53-502d-4639-8dd3-2e66c3750df8" />

## 5. Count how many places have a rating of 4 or higher
```sql
SELECT COUNT(*) FROM cleaned_file WHERE rating >= 4;
```
<img width="125" alt="Screenshot 1446-08-12 at 11 51 11 AM" src="https://github.com/user-attachments/assets/42553bf9-6fd9-4fa2-9b3f-32e0de4b72e7" />

## 6. Find locations with missing best_comment
```sql
SELECT name, location FROM cleaned_file WHERE best_comment IS NULL;
```
<img width="162" alt="Screenshot 1446-08-12 at 11 52 36 AM" src="https://github.com/user-attachments/assets/07be1302-b066-4a76-a5b4-529c764df834" />

## 7. select all with review_count > 9900
```sql
select  * from cleaned_file where review_count > 9900;
```
<img width="1117" alt="Screenshot 1446-08-12 at 11 54 26 AM" src="https://github.com/user-attachments/assets/d14cca75-f20b-4660-9e80-39fcbfdfcd22" />

## 8. Find the number of locations per genre
```sql
SELECT genre, COUNT(*) AS total FROM cleaned_file GROUP BY genre;
```
<img width="267" alt="Screenshot 1446-08-12 at 11 56 09 AM" src="https://github.com/user-attachments/assets/6a20a7b2-3500-4645-9e46-1a933b7550c7" />

## 9. Find the average rating for movie theaters
```sql
SELECT AVG(rating) FROM cleaned_file WHERE genre = ' Movie theater';
```
<img width="144" alt="Screenshot 1446-08-12 at 11 57 08 AM" src="https://github.com/user-attachments/assets/13c9d73b-c89c-4527-834f-a02482f43df3" />

## 10. Find all places located in Saudi Arabia
```sql
SELECT name, location FROM cleaned_file WHERE location LIKE '%Saudi Arabia%';
```
<img width="491" alt="Screenshot 1446-08-12 at 11 59 16 AM" src="https://github.com/user-attachments/assets/805a0dbd-f789-4fc5-9974-51b9e4146b6b" />


