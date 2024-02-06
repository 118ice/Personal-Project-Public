layout: page
title: "PAGE-TITLE"
permalink: /URL-PATH

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Maths Questions</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            display: flex;
        }
        
        #question-list {
            width: 200px;
            height: 100vh;
            overflow-y: scroll;
            border-right: 1px solid #ccc;
        }
        
        #question-list ul {
            list-style-type: none;
            padding: 0;
            margin: 0;
        }
        
        #question-list li {
            padding: 10px;
            cursor: pointer;
            transition: background-color 0.3s;
        }
        
        #question-list li:hover {
            background-color: #f0f0f0;
        }
        
        #question-area {
            flex: 1;
            padding: 20px;
        }
    </style>
</head>
<body>
    <div id="question-list">
        <ul>
            <li onclick="showQuestion(1)">Question 1</li>
            <li onclick="showQuestion(2)">Question 2</li>
            <li onclick="showQuestion(3)">Question 3</li>
            <li onclick="showQuestion(4)">Question 4</li>
            <li onclick="showQuestion(5)">Question 5</li>
            <!-- Add more questions as needed -->
        </ul>
    </div>
    <div id="question-area">
        <h1>Welcome to Maths Questions!</h1>
        <p>Select a question from the list on the left.</p>
        <div id="question-content">
            <!-- Question content will be loaded here -->
        </div>
    </div>

    <script>
        function showQuestion(questionNumber) {
            var questionContent = "";
            // You can replace the content below with your actual math questions
            switch (questionNumber) {
                case 1:
                    questionContent = "Question 1: What is 2 + 2?";
                    break;
                case 2:
                    questionContent = "Question 2: What is the square root of 16?";
                    break;
                case 3:
                    questionContent = "Question 3: What is 3 x 5?";
                    break;
                case 4:
                    questionContent = "Question 4: What is 10 - 7?";
                    break;
                case 5:
                    questionContent = "Question 5: What is 20 / 4?";
                    break;
                // Add more cases as needed
            }
            document.getElementById("question-content").innerHTML = questionContent;
        }
    </script>
</body>
</html>
