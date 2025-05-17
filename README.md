# Smart Flashcard Backend

This is a backend API for a smart flashcard system. It allows users to add flashcards without specifying the subject; the subject is inferred automatically based on the question text. Flashcards can be retrieved in a shuffled, mixed-subject format.

## Features

- Add flashcards with subject detection
- Retrieve flashcards by student, mixed by subject
- Rule-based or model-based subject classification

## Endpoints

### Add Flashcard

**POST** `/flashcard`

Request Body:
```json
{
  "student_id": "stu001",
  "question": "What is Newton's Second Law?",
  "answer": "Force equals mass times acceleration"
}
