<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Resume</title>
    <style>
        body {
            font-family: 'Helvetica Neue', Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f9;
            color: #333;
        }
        .container {
            max-width: 900px;
            margin: 50px auto;
            padding: 20px;
            background-color: #fff;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
            border-radius: 10px;
        }
        h1, h2 {
            text-align: center;
            color: #2c3e50;
        }
        .nav-buttons {
            text-align: center;
            margin-bottom: 30px;
        }
        .nav-buttons button {
            margin: 10px;
            padding: 10px 20px;
            font-size: 16px;
            border: none;
            border-radius: 5px;
            background-color: #3498db;
            color: white;
            cursor: pointer;
            transition: background-color 0.3s;
        }
        .nav-buttons button:hover {
            background-color: #2980b9;
        }
        .section {
            display: none;
            padding: 20px;
            border-top: 1px solid #ddd;
        }
        .section.active {
            display: block;
        }
        ul {
            padding-left: 20px;
            list-style-type: disc;
        }
        .footer {
            text-align: center;
            margin-top: 20px;
            font-size: 14px;
            color: #888;
        }
    </style>
    <script>
        function showSection(sectionId) {
            const sections = document.querySelectorAll('.section');
            sections.forEach(section => section.classList.remove('active'));
            document.getElementById(sectionId).classList.add('active');
        }
    </script>
</head>
<body>
    <div class="container">
        <h1>My Personal Information</h1>

        <div class="nav-buttons">
            <button onclick="showSection('myself')">Myself</button>
            <button onclick="showSection('family')">My Family</button>
            <button onclick="showSection('favorites')">My Favorites</button>
            <button onclick="showSection('resume')">My Resume</button>
        </div>

        <div id="myself" class="section active">
            <h2>Myself</h2>
            <p><strong>Name:</strong> Zeth Isaiah Mendoza</p>
            <p><strong>Date of Birth:</strong> 10/24/2006</p>
            <p><strong>Address:</strong> Blk 7 Lot 37 Malagasang 1-B Imus, Cavite, Celina Plains, Acacia Street</p>
        </div>

        <div id="family" class="section">
            <h2>My Family</h2>
            <p><strong>Mother:</strong> Laricell S. Mendoza</p>
            <p><strong>Father:</strong> Daniel Axam</p>
        </div>

        <div id="favorites" class="section">
            <h2>My Favorites</h2>
            <p><strong>Hobbies:</strong></p>
            <ul>
                <li>Playing instruments like Guitar and Ukulele</li>
                <li>Reading</li>
                <li>Playing Games</li>
                <li>Sports like Badminton and Volleyball</li>
                <li>Singing</li>
                <li>Eating</li>
                <li>Sleeping</li>
                <li>Cooking</li>
                <li>Watching Movies</li>
                <li>Watching Anime</li>
            </ul>
        </div>

        <div id="resume" class="section">
            <h2>My Resume</h2>
            <p>Motivated first-year <strong>BSCS</strong> student at <strong>CVSU Imus</strong>, eager to apply theoretical knowledge in Computer Science. Seeking opportunities to gain experience and develop skills in whatever opportunity that may arise.</p>
            <p><strong>Skills:</strong></p>
            <ul>
                <li><strong>Technical Skills:</strong> Proficient in Microsoft Word, PowerPoint, and Excel</li>
                <li><strong>Soft Skills:</strong> Communicator, Time Management, Team Collaboration</li>
                <li><strong>Languages:</strong> Fluent in English and Tagalog</li>
            </ul>
        </div>
    </div>
    </div>
</body>
</html>
