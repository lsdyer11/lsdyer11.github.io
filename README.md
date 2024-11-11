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

        select, input, button {
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
        <p>Select your grade, subject, and type a topic to get started.</p>
        
        <label for="grade">Grade:</label>
        <select id="grade">
            <option value="prek">Pre-K</option>
            <option value="k">Kindergarten</option>
            <option value="1">1st Grade</option>
            <option value="2">2nd Grade</option>
            <option value="3">3rd Grade</option>
            <option value="4">4th Grade</option>
            <option value="5">5th Grade</option>
            <option value="6">6th Grade</option>
            <option value="7">7th Grade</option>
            <option value="8">8th Grade</option>
            <option value="9">9th Grade</option>
            <option value="10">10th Grade</option>
            <option value="11">11th Grade</option>
            <option value="12">12th Grade</option>
        </select>

        <label for="subject">Subject:</label>
        <select id="subject">
            <option value="math">Math</option>
            <option value="science">Science</option>
            <option value="history">History</option>
            <option value="english">English</option>
            <option value="art">Art</option>
            <option value="music">Music</option>
            <option value="geography">Geography</option>
            <option value="computer_science">Computer Science</option>
            <option value="health">Health</option>
            <option value="economics">Economics</option>
        </select>

        <label for="topic">Topic:</label>
        <input type="text" id="topic" placeholder="Type your topic here">

        <button onclick="generateOverview()">Get Overview</button>

        <div id="output"></div>
    </div>

    <script>
        // Sample AI responses based on selected options
        const responses = {
            "8-math-algebra": "In 8th-grade Algebra, you’ll learn about solving equations, graphing linear functions, and understanding variables.",
            "8-science-biology": "In 8th-grade Biology, you’ll explore cell structures, human anatomy, and the basics of genetics.",
            "9-history-civil_war": "In 9th-grade History, learn about the causes and impact of the Civil War in American history.",
            "10-english-literature": "In 10th-grade English, you'll study literature, including novels, poetry, and plays from various authors.",
            // Add more responses as needed
        };

        function generateOverview() {
            const grade = document.getElementById("grade").value;
            const subject = document.getElementById("subject").value;
            const topic = document.getElementById("topic").value.trim().toLowerCase();
            const key = `${grade}-${subject}-${topic}`;
            
            const outputDiv = document.getElementById("output");
            if (responses[key]) {
                outputDiv.innerHTML = `<strong>Overview:</strong> ${responses[key]}`;
            } else {
                outputDiv.innerHTML = `Sorry, an overview is not available for "${topic}". Try another topic or check back later.`;
            }
        }
    </script>
</body>
</html>