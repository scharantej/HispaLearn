## Design for a Flask App to Learn Spanish Language

### HTML Files

- **index.html**: The main page of the application where users start their Spanish learning journey. This page will present various options for learning, such as lessons, exercises, and quizzes.
- **lesson.html**: A dedicated page that displays a specific Spanish lesson, including grammar explanations, vocabulary, and examples.
- **exercise.html**: A page for users to practice their Spanish skills through interactive exercises, such as fill-in-the-blanks, matching, or translation.
- **quiz.html**: A page that evaluates users' understanding of Spanish through a series of questions. The results of the quiz can be used to track progress and identify areas for improvement.

### Routes

- **@app.route('/')**: This route handles the request for the main page, displaying the **index.html** file.
- **@app.route('/lesson/<lesson_id>'**: This route displays a specific lesson when users click on a lesson from the main page. It takes the **lesson_id** as a parameter to determine which lesson to show and renders the **lesson.html** file with the corresponding lesson content.
- **@app.route('/exercise/<exercise_id>'**: Similar to the lesson route, this route handles requests for specific exercises. It takes the **exercise_id** as a parameter and renders the **exercise.html** file with the appropriate exercise content.
- **@app.route('/quiz/<quiz_id>'**: This route serves a specific quiz when users want to test their Spanish skills. It takes the **quiz_id** as a parameter to identify the quiz and renders the **quiz.html** file with the quiz questions.
- **@app.route('/submit_quiz', methods=['POST'])**: This route handles the submission of the quiz. It collects the user's answers and evaluates them against the correct answers to provide feedback and calculate the user's score.