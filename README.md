<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tarun Karigar - GitHub Profile</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap');
        
        body {
            font-family: 'Poppins', sans-serif;
            background: linear-gradient(to right, #141e30, #243b55);
            color: white;
            margin: 0;
            padding: 0;
            text-align: center;
        }
        .container {
            max-width: 90%;
            margin: 40px auto;
            background: rgba(255, 255, 255, 0.1);
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 0 15px rgba(0, 0, 0, 0.3);
        }
        h1, h2 {
            color: #ffcc00;
        }
        .profile-img {
            width: 120px;
            height: 120px;
            border-radius: 50%;
            border: 4px solid #ffcc00;
            margin-bottom: 10px;
        }
        .section {
            margin-top: 20px;
            padding: 20px;
            background: rgba(255, 255, 255, 0.2);
            border-radius: 10px;
        }
        ul {
            list-style: none;
            padding: 0;
        }
        li {
            padding: 15px;
            background: rgba(255, 255, 255, 0.3);
            border-radius: 8px;
            margin: 10px 0;
            cursor: pointer;
            transition: background 0.3s;
        }
        li:hover {
            background: rgba(255, 255, 255, 0.5);
        }
        a {
            color: #ffcc00;
            text-decoration: none;
            font-weight: bold;
        }
        a:hover {
            text-decoration: underline;
        }
        .btn {
            display: inline-block;
            padding: 12px 25px;
            margin: 10px;
            background: #ffcc00;
            color: #1e3c72;
            border-radius: 5px;
            text-decoration: none;
            font-weight: bold;
            transition: 0.3s;
        }
        .btn:hover {
            background: #e6b800;
        }
        .modal {
            display: none;
            position: fixed;
            z-index: 10;
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.8);
            padding-top: 80px;
        }
        .modal-content {
            background-color: white;
            color: black;
            margin: auto;
            padding: 20px;
            width: 70%;
            border-radius: 10px;
            text-align: left;
        }
        .close {
            color: red;
            float: right;
            font-size: 28px;
            font-weight: bold;
            cursor: pointer;
        }
        @media screen and (max-width: 600px) {
            .modal-content {
                width: 90%;
            }
            .btn {
                padding: 10px 20px;
            }
        }
    </style>
    <script>
        function showProjectDetails(details) {
            document.getElementById("modal-text").innerHTML = details;
            document.getElementById("projectModal").style.display = "block";
        }
        function closeModal() {
            document.getElementById("projectModal").style.display = "none";
        }
    </script>
</head>
<body>
    <div class="container">
        <img src="Tarun_img.JPG" alt="Tarun Karigar" class="profile-img">
        <h1>👋 Hello, I'm TARUN KARIGAR</h1>
        <p>Electronics and Communication Engineer | Embedded Systems | IoT | Java Developer</p>
        <a href="https://linktr.ee/tarunkarigar" class="btn" target="_blank">🌐 My Portfolio</a>

        <div class="section">
            <h2>🚀 About Me</h2>
            <p>🎓 Final-year ECE student at AGMR College of Engineering and Technology</p>
            <p>💻 Passionate about Embedded Systems, IoT, and Software Development</p>
            <p>🔍 Currently learning Advanced Java and PCB Design</p>
        </div>

        <div class="section">
            <h2>📌 Projects</h2>
            <ul>
                <li onclick="showProjectDetails('Optimized 8x8-bit SRAM array with power-efficient row decoder using Cadence Virtuoso, achieving 3.14mW power consumption.')">🧠 Design of an 8X8 Bit SRAM Array with Row Decoder</li>
                <li onclick="showProjectDetails('IoT-based restroom control system that automatically manages lavatory doors based on train proximity, improving hygiene and convenience.')">🚆 Train-Station Proximity Restroom Control System</li>
                <li onclick="showProjectDetails('Full-stack crop management system application with an intuitive user interface and seamless data management.')">🌱 Crop Management System Application</li>
            </ul>
        </div>

        <div class="section">
            <h2>📫 Let's Connect!</h2>
            <a href="mailto:tarunkarigar9@gmail.com" class="btn">💌 Email</a>
            <a href="https://www.linkedin.com/in/tarun-karigar" class="btn" target="_blank">🔗 LinkedIn</a>
            <a href="https://twitter.com/tarunkarigar" class="btn" target="_blank">🐦 X (Twitter)</a>
            <p>📞 Contact: 9972548514</p>
        </div>
    </div>

    <div id="projectModal" class="modal">
        <div class="modal-content">
            <span class="close" onclick="closeModal()">&times;</span>
            <p id="modal-text"></p>
        </div>
    </div>
</body>
</html>
