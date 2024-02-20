# Login-Page 
<style>
        .background-container {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -1;
            background: url(http://wallpapercave.com/wp/T5pc8RA.jpg) no-repeat;
            background-size: cover;
            background-position: center;
            animation: animateBg 5s linear infinite;
        }

        @keyframes animateBg {
            100% {
                filter: hue-rotate(360deg);
            }
        }
        body {
    font-family: Poppins, sans-serif;
    display: flex;
    align-items: center;
    justify-content: center;
    height: 100vh;
    margin: 0;
        }
.container {
    max-width: 400px;
    padding: 20px;
    border: 1px solid #ccc;
    border-radius: 5px;
    width: 130%;
        height: 50vh;
}

h2{
    font-size: 2em;
            color: #fff;
            text-align: center;
}

form {
    display: flex;
    flex-direction: column;
    width: 100%;
  
    }

label {
    margin-top: 10px;
    color: #fff;
}

input {
    padding: 8px;
    margin-top: 5px;
    margin-bottom: 10px;
    background: transparent;
    color:#fff;
}

button {
    background-color:red;
    color: white;
    padding: 10px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}
    </style>
</head>
<body>
    <div class="background-container"></div>
    <div class="container">
        <form id="loginForm">
            <h2>Login</h2>
            <label for="username">Username:</label>
            <input type="text" id="username" name="username" required>

            <label for="password">Password:</label>
            <input type="password" id="password" name="password" required>

            <!-- Change type to "button" -->
            <button type="button" onclick="validateLogin()">Login</button>
        </form>
    </div>
    <script>
        function validateLogin() {
    var username = document.getElementById("username").value;
    var password = document.getElementById("password").value;

    if (username == "showtime" && password == "1234") {
        window.location.href='home.html';
    } else {
        alert("Invalid username or password. Please try again.");
    }
}
    </script>
</body>
</html>
