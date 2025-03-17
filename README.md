<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Baseball Walk-Up Song Selector</title>
    <style>
        body {
            background: linear-gradient(135deg, #8B4513, #DAA520); /* Brown to yellow gradient */
            font-family: 'Arial', sans-serif;
            color: #FFF; /* White text */
            text-align: center;
            margin: 0;
            padding: 20px;
            animation: colorShift 10s infinite;
        }
        @keyframes colorShift {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }
        h1 {
            font-size: 3em;
            color: #DAA520; /* Yellow */
            text-shadow: 2px 2px #000; /* Black shadow for contrast */
            margin-bottom: 20px;
        }
        p {
            font-size: 1.2em;
            margin: 10px 0;
            color: #FFF; /* White */
        }
        .instructions {
            background-color: rgba(0, 0, 0, 0.3); /* Semi-transparent black */
            padding: 15px;
            border: 2px solid #DAA520; /* Yellow border */
            border-radius: 10px;
            margin: 20px auto;
            max-width: 600px;
        }
        #disqus_thread {
            background-color: rgba(139, 69, 19, 0.2); /* Light brown overlay */
            padding: 20px;
            border: 2px solid #000; /* Black border */
            border-radius: 10px;
            margin-top: 20px;
            max-width: 800px;
            margin-left: auto;
            margin-right: auto;
        }
        /* Button for lazy loading comments */
        .load-comments {
            background-color: #DAA520; /* Yellow */
            color: #000; /* Black text */
            padding: 10px 20px;
            border: 2px solid #000; /* Black border */
            border-radius: 5px;
            cursor: pointer;
            font-size: 1.1em;
        }
        .load-comments:hover {
            background-color: #FFD700; /* Lighter yellow on hover */
        }
    </style>
</head>
<body>
    <h1>Baseball Walk-Up Song Selector!</h1>
    <p>Get ready to pump up the crowd at the next game!</p>
    <div class="instructions">
        <p>Help us choose the best walk-up songs for our baseball hitters! Please leave a comment below suggesting <strong>two songs</strong> you’d love to hear as players step up to bat. Include the song titles and artists (e.g., "Sweet Child O' Mine" by Guns N' Roses and "Uptown Funk" by Mark Ronson ft. Bruno Mars).</p>
        <p>Let’s make every at-bat epic!</p>
    </div>
</body>
</html>
