<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>TRILCE - PLATAFORMA VIRTUAL</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }
    body {
      display: flex;
      min-height: 100vh;
      background: #f5f7fa;
    }
    .sidebar {
      width: 220px;
      background-color: #004080;
      color: white;
      display: flex;
      flex-direction: column;
      padding: 20px;
    }
    .sidebar h2 {
      font-size: 18px;
      margin-bottom: 30px;
      text-align: center;
    }
    .nav-link {
      display: flex;
      align-items: center;
      gap: 10px;
      padding: 12px;
      margin-bottom: 10px;
      border-radius: 5px;
      color: white;
      text-decoration: none;
      transition: background 0.3s;
    }
    .nav-link:hover {
      background-color: #0066cc;
    }
    .content {
      flex: 1;
      padding: 30px;
    }
    .section {
      display: none;
    }
    .active {
      display: block;
    }
    h2 {
      margin-bottom: 20px;
    }
    .dashboard-cards {
      display: flex;
      justify-content: space-around;
      margin-bottom: 30px;
    }
    .card {
      background: white;
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
      width: 50%;
      text-align: center;
    }
    table {
      width: 100%;
      border-collapse: collapse;
      background: white;
      border-radius: 10px;
      overflow: hidden;
    }
    th, td {
      padding: 12px;
      border: 1px solid #ccc;
      text-align: left;
    }
    .gallery{
      display: flex;
      gap: 20px;
      flex-wrap: wrap;
    }
    .gallery-item{
      flex: 1;
      width: 500px;
      background: white;
      padding: 20px;
      text-align: center;
      border-radius: 10px;
      box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    }
    .gallery-item img{
      width: 200px;
      margin-bottom: 10px;
    }

     .reports {
      display: flex;
      gap: 20px;
      flex-wrap: wrap;
    }
     .report-item {
      flex: 1;
      width: 500px;
      background: white;
      padding: 20px;
      text-align: center;
      border-radius: 10px;
      box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    }
     .report-item img {
      width: 50px;
      margin-bottom: 10px;
    }

    .contact-form {
      background: white;
      padding: 20px;
      border-radius: 10px;
      max-width: 600px;
      width: 100%;
    }
    .contact-form input,
    .contact-form textarea {
      width: 100%;
      padding: 10px;
      margin-bottom: 15px;
      border: 1px solid #ccc;
      border-radius: 5px;
    }
    .contact-form button {
      background-color: #004080;
      color: white;
      padding: 10px 20px;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }
    .footer {
      background-color: #00264d;
      color: white;
      text-align: center;
      padding: 15px;
      position: fixed;
      bottom: 0;
      width: 100%;
    }
  </style>
</head>
<body>
  <div class="sidebar">
    <h2>TRILCE - PLATAFORMA VIRTUAL</h2>
    <a href="#inicio" class="nav-link" onclick="showSection('inicio')">🏠 Inicio</a>
    <a href="#reportes" class="nav-link" onclick="showSection('reportes')">📊 Reportes</a>
    <a href="#galeria" class="nav-link" onclick="showSection('galeria')">🖼️ Galería</a>
    <a href="#contacto" class="nav-link" onclick="showSection('contacto')">📬 Contacto</a>
  </div>

  <div class="content">
    <div id="inicio" class="section active">
      <h2>Dashboard Académico</h2>
      <div class="dashboard-cards">
        <div class="card">
          <h3>Estudiantes</h3>
          <p>1500 Registrados</p>
        </div>
        <div class="card">
          <h3>Profesores</h3>
          <p>90 Activos</p>
        </div>
        <div class="card">
          <h3>Cursos</h3>
          <p>50 Disponibles</p>
        </div>
      </div>
      <h3>Información Académica</h3>
      <table>
        <thead>
          <tr><th>Curso</th><th>Profesor</th><th>Horario</th></tr>
        </thead>
        <tbody>
          <tr><td>Lenguaje</td><td>Lic. Herrera</td><td>8:00 - 9:50</td></tr>
          <tr><td>Historia</td><td>Lic. Ramírez</td><td>10:10 - 12:00</td></tr>
          <tr><td>Biología</td><td>Dr. Salazar</td><td>13:00 - 15:00</td></tr>
        </tbody>
      </table>
    </div>

    <div id="reportes" class="section">
      <h2>Reportes Académicos</h2>
      <div class="reports">
        <div class="report-item">
          <img src="RECURSOS/ASISTENCIAA.png" alt="Asistencia">
          <h4>Asistencia</h4>
          <p>Promedio del semestre actual</p>
        </div>
        <div class="report-item">
          <img src="RECURSOS/CALIFCIACIONES.png" alt="Calificaciones">
          <h4>Calificaciones</h4>
          <p>Resumen de calificaciones y promedios</p>
        </div>
        <div class="report-item">
          <img src="RECURSOS/MATRICULA.png" alt="Matrícula">
          <h4>Matrícula</h4>
          <p>Estado de matrícula estudiantil</p>
        </div>
      </div>
    </div>

    <div id="galeria" class="section">
      <h2>Galería Académica</h2>
      <div class="gallery">
        <div class="gallery-item">
          <h4>Conferencia 2025</h4>
          <img src="RECURSOS/CONFERENCIA.png" alt="Conferencia">
        </div>
        <div class="gallery-item">
          <h4>Graduación 2025</h4>
          <img src="RECURSOS/GRADUACION.jpeg" alt="GRADUACION">
        </div>
        <div class="gallery-item">
          <h4>Feria de Ciencia</h4>
          <img src="RECURSOS/FERIA.jpeg" alt="FERIA DE CIENCIA">
        </div>
      </div>
    </div>

    <div id="contacto" class="section">
      <h2>Contacto</h2>
      <div class="contact-form">
        <form action="https://trilce.ucv.edu.pe/default.aspx" method="get">
          <input type="text" name="nombre" placeholder="Tu nombre" required>
          <input type="email" name="email" placeholder="Correo electrónico" required>
          <textarea name="mensaje" placeholder="Escribe tu mensaje" required></textarea>
          <button type="submit">Enviar</button>
        </form>
      </div>
    </div>
  </div>

  <div class="footer">
    INTEGRANTES:<br>
    - GALVEZ ZUÑIGA SOFIA NICOLL<br>
    - PALOMINO BARRIOS LUZ MERY
  </div>

  <script>
    function showSection(id) {
      document.querySelectorAll('.section').forEach(sec => sec.classList.remove('active'));
      document.getElementById(id).classList.add('active');
    }
  </script>
</body>
</html>
