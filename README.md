- 👋 Hi, I’m @Alphapellel624
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
Alphapellel624/Alphapellel624 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your <?php
include("config.php");

// Vérifier si le formulaire est soumis
if ($_SERVER["REQUEST_METHOD"] == "POST") {
    $name = $_POST["name"];
    $email = $_POST["email"];

    $sql = "INSERT INTO users (name, email) VALUES ('$name', '$email')";

    if ($conn->query($sql) === TRUE) {
        echo "Nouvel utilisateur ajouté avec succès !<br>";
        echo "<a href='index.php'>Voir la liste des utilisateurs</a>";
    } else {
        echo "Erreur : " . $conn->error;
    }
}

$conn->close();
?>

<!DOCTYPE html>
<html>
<head>
    <title>koneedi</title>
</head>
<body>
    <h1>Ajouter un utilisateur</h1>
    <form method="POST" action="">
        <label>Nom :</label><br>
        <input type="text" name="name" required><br><br>

        <label>Email :</label><br>
        <input type="email" name="email" required><br><br>

        <input type="submit" value="Ajouter">
    </form>
</body>
</html>

