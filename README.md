<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Social Media handles</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            overflow: hidden; /* Prevent scrolling */
        }
        .video-background {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: 1;
        }
        iframe {
            width: 100%;
            height: 100%;
            border: none;
        }
        .overlay {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            display: flex;
            justify-content: center;
            align-items: center;
            z-index: 2;
            background: rgba(0, 0, 0, 0.5); /* Semi-transparent overlay for readability */
        }
        .social-links {
            display: flex;
            flex-wrap: wrap;
            gap: 30px;
            justify-content: center;
        }
        .social-link {
            display: flex;
            flex-direction: column;
            align-items: center;
            text-decoration: none;
            color: #fff;
            transition: transform 0.2s;
            background: rgba(0, 0, 0, 0.7);
            padding: 20px;
            border-radius: 10px;
        }
        .social-link:hover {
            transform: scale(1.1);
        }
        .social-logo {
            width: 60px;
            height: 60px;
            margin-bottom: 10px;
        }
        h1 {
            margin-bottom: 20px;
            font-size: 2em;
        }
    </style>
</head>
<body>
    <div class="video-background">
        <iframe id="carVideo" src="" allowfullscreen></iframe>
    </div>
    
    <div class="overlay">
        <div>
            <h1>Welcome to My Page</h1>
            <p>Check out my social media!</p>
            <div class="social-links">
                <a href="https://www.instagram.com/the_shy_boy_07?igsh=MWg3aGU0YjloZ2llZw==" target="_blank" class="social-link">
                    <img src="https://cdn.jsdelivr.net/npm/simple-icons@v9/icons/instagram.svg" alt="Instagram" class="social-logo">
                    Instagram
                </a>
                <a href="https://twitter.com/yourhandle" target="_blank" class="social-link">
                    <img src="https://cdn.jsdelivr.net/npm/simple-icons@v9/icons/twitter.svg" alt="Twitter" class="social-logo">
                    Twitter
                </a>
                <a href="https://youtube.com/yourhandle" target="_blank" class="social-link">
                    <img src="https://cdn.jsdelivr.net/npm/simple-icons@v9/icons/youtube.svg" alt="YouTube" class="social-logo">
                    YouTube
                </a>
                <a href="https://linkedin.com/in/yourhandle" target="_blank" class="social-link">
                    <img src="https://cdn.jsdelivr.net/npm/simple-icons@v9/icons/linkedin.svg" alt="LinkedIn" class="social-logo">
                    LinkedIn
                </a>
            </div>
        </div>
    </div>
    
    <script>
        // Array of 4K car video YouTube embed URLs (randomly selected)
        const carVideos = [
            "https://www.youtube.com/embed/8pP2zNJG6rE?autoplay=1&mute=1&loop=1&playlist=8pP2zNJG6rE", // Ferrari 488 Spider 4K
            "https://www.youtube.com/embed/6pN9W9nZvQw?autoplay=1&mute=1&loop=1&playlist=6pN9W9nZvQw", // Lamborghini Huracan 4K
            "https://www.youtube.com/embed/7nOb8UBPOhE?autoplay=1&mute=1&loop=1&playlist=7nOb8UBPOhE", // McLaren 720S 4K
            "https://www.youtube.com/embed/9bZkp7q19f0?autoplay=1&mute=1&loop=1&playlist=9bZkp7q19f0", // Porsche 911 GT3 4K
            "https://www.youtube.com/embed/M7ZMz6K8mEM?autoplay=1&mute=1&loop=1&playlist=M7ZMz6K8mEM",  // Bugatti Chiron 4K
            "https://www.youtube.com/embed/vRPC64KVkGg?autoplay=1&mute=1&loop=1&playlist=vRPC64KVkGg"  // Your added YouTube Short
        ];
        
        // Function to select a random video
        function loadRandomVideo() {
            const randomIndex = Math.floor(Math.random() * carVideos.length);
            document.getElementById('carVideo').src = carVideos[randomIndex];
        }
        
        // Load a random video on page load
        window.onload = loadRandomVideo;
    </script>
</body>
</html>
