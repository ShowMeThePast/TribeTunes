<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Baseball Walk-Up Song Selector</title>
    <style>
        body {
            background: linear-gradient(135deg, #ff6f61, #6b48ff, #ffeb3b);
            font-family: 'Arial', sans-serif;
            color: #fff;
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
            color: #ffeb3b;
            text-shadow: 2px 2px #6b48ff;
            margin-bottom: 20px;
        }
        p {
            font-size: 1.2em;
            margin: 10px 0;
            color: #fff;
        }
        .instructions {
            background-color: rgba(255, 255, 255, 0.1);
            padding: 15px;
            border-radius: 10px;
            margin: 20px auto;
            max-width: 600px;
        }
        #disqus_thread {
            background-color: rgba(255, 255, 255, 0.2);
            padding: 20px;
            border-radius: 10px;
            margin-top: 20px;
            max-width: 800px;
            margin-left: auto;
            margin-right: auto;
        }
        /* Button for lazy loading comments */
        .load-comments {
            background-color: #ff6f61;
            color: #fff;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 1.1em;
        }
        .load-comments:hover {
            background-color: #e65b50;
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

    <button class="load-comments" onclick="loadComments()">Load Comments</button>
    <div id="disqus_thread"></div>

    <script>
        function loadComments() {
            var disqus_config = function () {
                this.page.url = "https://showmethepast.github.io/TribeTunes/"; // Replace with your GitHub Pages URL
                this.page.identifier = "walk-up-songs";
                this.page.title = "Baseball Walk-Up Song Selector";
            };

            var d = document, s = d.createElement('script');
            s.src = 'https://<your-disqus-shortname>.disqus.com/embed.js';
            s.setAttribute('data-timestamp', +new Date());
            (d.head || d.body).appendChild(s);

            // Hide the button after loading
            document.querySelector('.load-comments').style.display = 'none';
        }
    </script>
</body>
</html>
