<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AI Study Helper</title>
    <style>
        /* Basic styling */
        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            margin: 0;
            background-color: #f5f5f5;
        }

        .container {
            text-align: center;
            max-width: 500px;
            padding: 20px;
            background-color: #fff;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }

        select, button {
            margin: 10px 0;
            padding: 10px;
            font-size: 1em;
            width: 100%;
        }

        #output {
            margin-top: 20px;
            padding: 15px;
            background-color: #e0f7fa;
            border-radius: 5px;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>AI Study Helper</h1>
        <p>Select your grade, subject, and topic to get started.</p>
        
        <label for="grade">Grade:</label>
        <select id="grade">
            <option value="8">8th Grade</option>
            <option value="9">9th Grade</option>
            <option value="10">10th Grade</option>
        </select>

        <label for="subject">Subject:</label>
        <select id="subject">
            <option value="math">Math</option>
            <option value="science">Science</option>
            <option value="history">History</option>
        </select>

        <label for="topic">Topic:</label>
        <select id="topic">
            <option value="algebra">Algebra</option>
            <option value="biology">Biology</option>
            <option value="civil_war">Civil War</option>
        </select>

        <button onclick="generateOverview()">Get Overview</button>

        <div id="output"></div>
    </div>

    <script>
        // Sample AI responses based on selected options
        const responses = {
            "8-math-algebra": "In 8th-grade Algebra, you’ll learn about solving equations, graphing linear functions, and understanding variables.",
            "8-science-biology": "In 8th-grade Biology, you’ll explore cell structures, human anatomy, and the basics of genetics.",
            "8-history-civil_war": "In 8th-grade History, learn about the causes and impact of the Civil War in American history.",
            "9-math-algebra": "In 9th-grade Algebra, you’ll dive into quadratic equations, polynomials, and more advanced functions.",
            // Add more responses as needed
        };

        function generateOverview() {
            const grade = document.getElementById("grade").value;
            const subject = document.getElementById("subject").value;
            const topic = document.getElementById("topic").value;
            const key = `${grade}-${subject}-${topic}`;
            
            const outputDiv = document.getElementById("output");
            if (responses[key]) {
                outputDiv.innerHTML = `<strong>Overview:</strong> ${responses[key]}`;
            } else {
                outputDiv.innerHTML = "Sorry, an overview is not available for this topic.";
            }
        }
    </script>
</body>
</html>