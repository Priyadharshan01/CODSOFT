# CODSOFT
online_internship_CODSOFT


PROJECT 1 LOGIN IN PAGE CREDENTIALS USING HTML AND CSS

<!DOCTYPE html>
<html>
<head>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f5f5f5;
    }

    .signup-container {
      max-width: 300px;
      margin: 0 auto;
      background-color: #fff;
      padding: 20px;
      border-radius: 5px;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    }

    h1 {
      text-align: center;
    }

    input, button {
      display: block;
      width: 100%;
      margin: 10px 0;
      padding: 10px;
      border: 1px solid #ccc;
      border-radius: 3px;
    }

    button {
      background-color: #007bff;
      color: #fff;
      border: none;
      cursor: pointer;
    }

    button:hover {
      background-color: #0056b3;
    }
  </style>
</head>
<body>
  <div class="signup-container">
    <h1>Sign Up</h1>
    <form id="signup-form" onsubmit="validateForm(event)">
      <input type="text" id="username" placeholder="Username" required>
      <input type="email" id="email" placeholder="Email" required>
      <input type="password" id="password" placeholder="Password" required>
      <button type="submit">Sign Up</button>
    </form>
  </div>
  <script>
    function validateForm(event) {
      event.preventDefault();

      const username = document.getElementById('username').value;
      const email = document.getElementById('email').value;
      const password = document.getElementById('password').value;

      if (username.trim() === '' || email.trim() === '' || password.trim() === '') {
        alert('Please fill in all fields');
      } else {
        // Perform your signup process here (e.g., sending data to a server).
        alert('Signup successful!');
        document.getElementById('signup-form').reset();
      }
    }
  </script>
</body>
</html>

