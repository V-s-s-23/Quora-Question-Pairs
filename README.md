# Quora-Question-Pairs

# Dataset Link :- https://www.kaggle.com/c/quora-question-pairs

# About Dataset :- Quora is a platform for Q&A, just like StackOverflow. But quora is more of a general-purpose Q&A platform that means there is not much code like in StackOverflow.

One of the many problems that quora face is the duplication of questions. Duplication of question ruins the experience for both the questioner and the answerer. Since the questioner is asking a duplicate question, we can just show him/her the answers to the previous question. And the answerer doesn’t have to repeat his/her answer for essentially the same questions.

For example, we have a question like “How can I be a good geologist?” and there are some answers to that question. Later someone else asks another question like “What should I do to be a great geologist?”.
We can see that both the questions are asking the same thing. Even though the wordings for the question are different, the intention of both questions is the same.
So the answers will be the same for both questions. That means we can just show the answers to the first question. That way the person who is asking the question will get the answers immediately and people who have answered already the first question don’t have to repeat themselves.

# Data Overview ->
Available Columns: id, qid1, qid2, question1, question2, is_duplicate
Class labels: 0, 1
Total training data / No. of rows: 404290
No. of columns: 6
is_duplicate is the dependent variable.
No. of non-duplicate data points is 255027
No. of duplicate data points is 149263

# EDA :- 

1. Common words ->

  ![download](https://user-images.githubusercontent.com/103623927/173188171-9b79fb79-fe26-496b-bb80-a3e3fefc4206.png)
  
   we can see if words in question1 and question2 are less than 4 , there is high probability that it will be "NON DUPLICATE" or if it more than 4 , there is high          probability it will be"Duplicate"

2. Total words:-

![download (1)](https://user-images.githubusercontent.com/103623927/173188318-8b378a77-a5cb-4b02-a0f6-2b651dc9c7db.png)

If total_word is in range 0-25 their is high chance it will be duplicate or if total words are more than 25 their is high chance it will be non_duplicate.

3. Words share:-

![download (2)](https://user-images.githubusercontent.com/103623927/173188407-048c2792-5f04-4885-b7df-35d6b7cc92d9.png)

we can see if word_share in question1 and question2 are less than 0.2 , there is high probability that it will be "NON DUPLICATE"
 or if it more than 0.2 , there is high probability it will be"Duplicate"
