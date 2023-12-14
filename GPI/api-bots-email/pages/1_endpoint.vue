<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Formulario de Correo - Alloxentric</title>
  <style>
    * {
      box-sizing: border-box;
    }
    body {
      font-family: 'Arial', sans-serif;
      margin: 0;
      padding: 0;
      display: flex;
    }
    .sidebar {
      background-color: #07b8b2;
      color: white;
      width: 250px;
      height: 100vh;
      padding: 20px;
    }
    .sidebar h2, .sidebar ul {
      margin: 0;
      padding: 0;
    }
    .sidebar ul {
      list-style: none;
    }
    .sidebar ul li {
      padding: 10px;
      cursor: pointer;
    }
    .sidebar ul li:hover {
      background-color: #066a62;
    }
    .main {
      flex-grow: 1;
      padding: 20px;
      background-color: #f4f4f4;
    }
    .main header, .main nav {
      background-color: #07b8b2;
      color: white;
    }
    .main header {
      padding: 10px 20px;
      text-align: center;
    }
    .main nav {
      display: flex;
      justify-content: space-around;
      padding: 10px 0;
    }
    .main nav a {
      color: white;
      text-decoration: none;
    }
    form {
      background-color: white;
      padding: 20px;
      margin-top: 20px;
    }
    label {
      margin-top: 10px;
    }
    input[type="email"], input[type="text"], textarea {
      width: 100%;
      padding: 8px;
      margin-top: 5px;
      border: 1px solid #ccc;
      border-radius: 4px;
    }
    input[type="submit"], button {
      background-color: #07b8b2;
      color: white;
      padding: 10px;
      border: none;
      border-radius: 4px;
      cursor: pointer;
      margin-top: 20px;
    }
    input[type="submit"]:hover, button:hover {
      background-color: #066a62;
    }
    .footer-bar {
      background-color: #07b8b2;
      color: white;
      padding: 10px 0;
      position: fixed;
      bottom: 0;
      left: 250px; /* Same as sidebar width */
      right: 0;
    }
  </style>
</head>
<body>
  <div class="sidebar">
    <h2>Alloxentric</h2>
    <ul>
      <li>Campañas</li>
      <li>Canales</li>
      <li>Bots</li>
      <li>Agentes</li>
      <li>Supervisión de Agentes</li>
      <li>MarketPlace</li>
      <li>Listas</li>
      <li>Dashboard</li>
      <li>Usuarios</li>
      <li>Consultas gmail</li>
    </ul>
  </div>
  <div class="main">
    <header>
      <h1>Formulario de Correo - Alloxentric</h1>
    </header>
    <nav>
      <a href="/">Inicio</a>
      <a href="/inbox">Bandeja de Entrada</a>
      <a href="/sent">Enviados</a>
      <a href="/drafts">Borradores</a>
    </nav>
    <form action="enviar.php" method="post">
      <label for="email">Tu correo:</label>
      <input type="email" id="email" name="email" required>

      <label for="asunto">Asunto:</label>
      <input type="text" id="asunto" name="asunto" required>

      <label for="mensaje">Mensaje:</label>
      <textarea id="mensaje" name="mensaje" required></textarea>

      <input type="submit" value="Enviar">
    </form>
    <h2>Bandeja de entrada</h2>
    <button id="refresh">Actualizar bandeja</button>
    <!-- Aquí se mostrarán los correos recibidos -->
  </div>
  <div class="footer-bar">
    <!-- Footer content -->
  </div>
</body>
</html>
