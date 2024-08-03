<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>@akkacjacodes GitHub Profile</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #0d1117;
            color: #c9d1d9;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }
        .container {
            text-align: center;
            max-width: 800px;
        }
        h1 {
            font-size: 3em;
            margin-bottom: 0.5em;
            opacity: 0;
            animation: fadeIn 1s ease-out forwards;
        }
        .subtitle {
            font-size: 1.5em;
            margin-bottom: 1em;
            opacity: 0;
            animation: fadeIn 1s ease-out 0.5s forwards;
        }
        .stats {
            display: flex;
            justify-content: space-around;
            margin-top: 2em;
        }
        .stat {
            opacity: 0;
            animation: fadeIn 1s ease-out 1s forwards;
        }
        .languages {
            margin-top: 2em;
        }
        .language {
            display: inline-block;
            margin: 0.5em;
            padding: 0.5em 1em;
            background-color: #21262d;
            border-radius: 5px;
            opacity: 0;
            animation: fadeIn 1s ease-out 1.5s forwards;
        }
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Hi there, I'm @akkacjacodes! 👋</h1>
        <p class="subtitle">Welcome to my GitHub profile!</p>
        <div class="stats">
            <div class="stat">
                <h3>Repositories</h3>
                <p id="repoCount">Loading...</p>
            </div>
            <div class="stat">
                <h3>Followers</h3>
                <p id="followerCount">Loading...</p>
            </div>
            <div class="stat">
                <h3>Contributions</h3>
                <p id="contributionCount">Loading...</p>
            </div>
        </div>
        <div class="languages">
            <span class="language">JavaScript</span>
            <span class="language">Python</span>
            <span class="language">React</span>
            <span class="language">Node.js</span>
        </div>
    </div>

    <script>
        // Simulated data loading (replace with actual API calls)
        setTimeout(() => {
            document.getElementById('repoCount').textContent = '25';
            document.getElementById('followerCount').textContent = '100';
            document.getElementById('contributionCount').textContent = '500+';
        }, 2000);
    </script>
</body>
</html>
