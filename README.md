<!DOCTYPE html>
<html>
    <meta charset="UTF-8"lang="en">
<head>meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My CV</title>
    <style>
        /* Your CSS styles here */

        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
        }

        .container {
            display: flex;
            max-width: 500px;
            margin: 100 auto;
        }

        .left-side {
            flex: 1;
            padding: 100px; /* Increased padding for more space */
            color: #fff; /* White text color for the left side */
            text-align: left;
            background: radial-gradient(circle at top left, #87CEEB 60%, transparent 60%), #041A40; /* Circular blue background for the upper part */
            background-size: 100% 100%, 100% 40%; /* Adjust the background sizes */
            background-repeat: no-repeat;
        }

        .photo {
            display: block;
            margin: 30px auto; /* Increased margin for more space */
            max-width: 150px;
            border-radius: 50%; /* Makes the photo circular */
        }

        .right-side {
            flex: 2;
            padding: 60px; /* Increased padding for more space */
            background-color: #fff;
        }

        h1 {
            margin: 0;
        }

        .personal-info {
            margin-bottom: 40px; /* Increased margin for more space */
        }

        .section {
            margin-bottom: 50px; /* Increased margin for more space */
        }

        .section h2 {
            color: #0074D9; /* Blue color for section titles */
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="left-side">
            <h1>Salah Jamal</h1>
            <img src="45.jpg" alt="Salah Jamal's Photo" class="photo">
            <div class="personal-info">
                <p>Email: salah@example.com</p>
                <p>Phone: (123) 456-7890</p>
                <p>Address: 123 Main St, City, Country</p>
            </div>
        </div>
        <div class="right-side">
            <h2>Enter Your Information</h2>
            <form action="generate_cv.php" method="POST">
                <label for="name">Name:</label>
                <input type="text" id="name" name="name" required><br><br>
                
                <label for="email">Email:</label>
                <input type="email" id="email" name="email" required><br><br>
                
                <label for="phone">Phone:</label>
                <input type="tel" id="phone" name="phone" required><br><br>
                
                <label for="address">Address:</label>
                <input type="text" id="address" name="address" required><br><br>
                
                <input type="submit" value="Generate CV">
            </form>
        </div>
    </div>
</body>
</html>
