<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Prueba de Envío de Correo Electrónico</title>
  <style>
    /* Estilos previamente definidos para sidebar, main, header, footer, etc. */
    /* ... */
    
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
      background-color: #f4f4f4;
      padding: 20px;
    }
    .main header {
      background-color: #07b8b2;
      color: white;
      padding: 10px 20px;
      text-align: center;
    }
    form {
      background-color: white;
      padding: 20px;
      margin-top: 20px;
    }
    label {
      margin-top: 10px;
    }
    input[type="text"], textarea {
      width: 100%;
      padding: 8px;
      margin-top: 5px;
      border: 1px solid #ccc;
      border-radius: 4px;
    }
    input[type="submit"] {
      background-color: #07b8b2;
      color: white;
      padding: 10px;
      border: none;
      border-radius: 4px;
      cursor: pointer;
      margin-top: 20px;
    }
    input[type="submit"]:hover {
      background-color: #066a62;
    }
    .footer-bar {
      background-color: #07b8b2;
      color: white;
      padding: 10px 0;
      position: fixed;
      bottom: 0;
      left: 250px; /* Same as sidebar width */
      width: calc(100% - 250px); /* Adjust width considering sidebar */
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
      <h1>Prueba de Envío de Correo Electrónico</h1>
    </header>
    <form id="email-test-send-form" method="post">
      <label for="correoPrueba">Correo de Prueba:</label>
      <input type="text" id="correoPrueba" name="correoPrueba" required>

      <label for="contenidoPrueba">Contenido del Correo de Prueba:</label>
      <textarea id="contenidoPrueba" name="contenidoPrueba" required></textarea>

      <label for="asuntoPrueba">Asunto del Correo de Prueba:</label>
      <input type="text" id="asuntoPrueba" name="asuntoPrueba">

      <label for="destinatarioPrueba">Destinatario del Correo de Prueba:</label>
      <input type="text" id="destinatarioPrueba" name="destinatarioPrueba">

      <input type="submit" value="Realizar Prueba de Envío">
    </form>
  </div>
  <div class="footer-bar">
    <!-- Contenido del pie de página -->
  </div>
</body>
</html>
