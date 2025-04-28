<!DOCTYPE html>

<html lang="en">

<head>

    <meta charset="UTF-8">

    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Attention please give answer</title>

    <style>

        body {

            font-family: Arial, sans-serif;

            text-align: center;

            background-color: #fafafa;

            margin: 0;

            padding: 0;

        }

        .container {

            width: 80%;

            margin: 40px auto;

            background-color: #f0f0f0;

            padding: 20px;

            border: 1px solid #ddd;

            border-radius: 10px;

            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);

        }

        .button {

            background-color: #4CAF50;

            color: #fff;

            padding: 10px 20px;

            border: none;

            border-radius: 5px;

            cursor: pointer;

            margin: 10px;

        }

        .button:hover {

            background-color: #3e8e41;

        }

        h1 {

            font-size: 24px;

            color: #333;

        }

        p {

            font-size: 18px;

            color: #555;

        }

        #answer {

            margin-top: 20px;

            font-size: 20px;

            color: #007BFF;

        }

    </style>

</head>

<body>

    <div class="container">

        <h1>Do You Love Me? 💕</h1>

        <p id="question"></p>

        <button id="yes" class="button">Yes</button>

        <button id="no" class="button">No</button>

        <p id="answer"></p>

    </div>

    <script>

        let question = document.getElementById("question");

        let yesButton = document.getElementById("yes");

        let noButton = document.getElementById("no");

        let answer = document.getElementById("answer");

        let questions = [

            "Do you love me? 💕",

            "Aise bhi kya baat hain kah do ji ? ❤️",

            "Are bol do haa usme kya sochna ? 😍"

        ];

        let currentQuestion = 0;

        question.innerHTML = questions[currentQuestion];

        yesButton.addEventListener("click", function() {

            answer.innerHTML = "Thanks! 😊 Mein janta hi tha musti ji aap karti ho 😅🥰";

        });

        noButton.addEventListener("click", function() {

            currentQuestion++;

            if (currentQuestion >= questions.length) {

                currentQuestion = 0;

            }

            question.innerHTML = questions[currentQuestion];

            answer.innerHTML = "";

        });

    </script>

</body>

</html>


