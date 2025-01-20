# Aryanpal
cybersequrity project 
<html>
<head>
<title>Password Manager - Add Password</title>
<link rel="stylesheet" href="style1.css">
</head>
<body>
<header>
<div class="container">
<h1 class="logo">Password Manager</h1>
<nav>
<ul class="nav-links">
<li><a href="index.html">Home</a></li>
<li><a href="add_password.html">Add Password</a></li>
<li><a href="view_passwords.html">View Passwords</a></li>
</ul>
</nav>
</div>
</header>
<main>
<section class="hero">
<div class="container">
<h2>Add Password</h2>
<form method="POST">
<label for="website">Website:</label>
<input type="text" name="website" required><br><br>
<label for="username">Username:</label>
<input type="text" name="username" required><br><br>
<label for="password">Password:</label>
<input type="password" name="password" id="password"
<input type="button" value="Generate"
required>
onclick="generatePassword(12)"><br><br>
<input type="submit" value="Add Password">
</form>
</div>
</section>
</main>
<script>
function generatePassword(length) {
var result
var characters
= '';
=
'ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789!@#$%^&*()_+
';
var charactersLength = characters.length;
for ( var i = 0; i < length; i++ ) {
result += characters.charAt(Math.floor(Math.random() *
charactersLength));
}
document.getElementById("password").value = result;
}
</script>
</body>
</html>
