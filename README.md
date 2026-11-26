<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Website</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f7f6;
            color: #333;
            margin: 0;
            padding: 0;
        }
        header {
            background-color: #2c3e50;
            color: white;
            text-align: center;
            padding: 30px 10px;
        }
        nav {
            background-color: #34495e;
            padding: 10px;
            text-align: center;
        }
        nav a {
            color: white;
            text-decoration: none;
            margin: 0 15px;
            font-weight: bold;
        }
        nav a:hover {
            text-decoration: underline;
        }
        .container {
            max-width: 800px;
            margin: 20px auto;
            background: white;
            padding: 25px;
            border-radius: 8px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }
        h2 {
            color: #2c3e50;
            border-bottom: 2px solid #eee;
            padding-bottom: 5px;
        }
        .profile-box {
            text-align: center;
            margin-bottom: 20px;
        }
        .profile-pic {
            width: 140px;
            height: 140px;
            border-radius: 50%;
            object-fit: cover;
            border: 3px solid #2c3e50;
        }
        .box {
            background: #eef2f3;
            padding: 15px;
            margin-top: 10px;
            border-radius: 5px;
        }
        /* Form Styling */
        form {
            display: flex;
            flex-direction: column;
            gap: 10px;
            margin-top: 10px;
        }
        input, textarea {
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
            font-size: 14px;
            font-family: Arial, sans-serif;
        }
        button {
            background-color: #27ae60;
            color: white;
            border: none;
            padding: 12px 20px;
            font-size: 16px;
            border-radius: 5px;
            cursor: pointer;
            width: fit-content;
        }
        button:hover {
            background-color: #219150;
        }
        footer {
            text-align: center;
            padding: 15px;
            background-color: #2c3e50;
            color: white;
            margin-top: 30px;
            font-size: 14px;
        }
    </style>
</head>
<body>

    <header>
        <h1>Swagat Hai Meri Website Par!</h1>
        <p>Ye mera pehla web development project hai.</p>
    </header>

    <nav>
        <a href="#about">Mere Baare Mein</a>
        <a href="#hobbies">Hobbies</a>
        <a href="#contact">Contact</a>
    </nav>

    <div class="container">
        <section id="about">
            <div class="profile-box">
                <!-- Apni photo ka naam yahan likhein -->
                <img src="meriphoto.jpg" alt="Meri Photo" class="profile-pic">
            </div>
            <h2>Mere Baare Mein</h2>
            <p>Namaste! Mera naam <b>[Apna Naam Likhein]</b> hai. Main abhi HTML aur CSS seekh raha hoon aur ye website maine khud code karke banayi hai.</p>
        </section>

        <section id="hobbies">
            <h2>Meri Hobbies</h2>
            <div class="box">
                <ul>
                    <li>Nayi cheezein seekhna aur coding karna</li>
                    <li>Music sunna aur movies dekhna</li>
                    <li>Doston ke saath ghoomna</li>
                </ul>
            </div>
        </section>

        <section id="contact">
            <h2>Contact Karein</h2>
            <p>Mujhe message bhejne ke liye neeche form bharein:</p>
            <form onsubmit="alert('Dhanyavaad! Aapka message mil gaya hai.'); return false;">
                <input type="text" placeholder="Aapka Naam" required>
                <input type="email" placeholder="Aapka Email" required>
                <textarea rows="4" placeholder=hey..." required></textarea>
                <button type="submit">Message Bhejein</button>
            </form>
        </section>
    </div>

    <footer>
        <p>Created by Golu kumar| 2026</p>
    </footer>

</body>
</html>
