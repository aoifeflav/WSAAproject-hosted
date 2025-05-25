<div class="container mt-5">
  <h1> Country Visits Tracker</h1>

  <p><strong>Module:</strong> Web Services and Applications<br>
     <strong>Author:</strong> Aoife Flavin<br>
     <strong>Student No:</strong> G00439331<br>
     <strong>Live Site:</strong> 
     <a href="https://aoifeflav.pythonanywhere.com/countryviewer.html" target="_blank">https://aoifeflav.pythonanywhere.com/countryviewer.html</a>
  </p>

  <h2>Overview</h2>
  <p>This is a personal web application developed as part of the <em>Web Services and Applications</em> module. It allows users to maintain a list of countries they have visited. Each entry includes the country name, date of visit, and a personal rating out of 10>.</p>
  <ul>
    <li><strong>Create</strong> a new country entry</li>
    <li><strong>Read</strong> and display all visited countries</li>
    <li><strong>Update</strong> country details</li>
    <li><strong>Delete</strong> a country entry</li>
  </ul>

  <h2>Technologies Used</h2>
  <ul>
    <li><a href="https://www.python.org/"><strong>Python (Flask)</strong> – Web framework for API routing</a></li>
    <li><a href="https://www.mysql.com/"><strong>MySQL</strong> – Relational database for data persistence</a></li>
    <li><a href="https://jquery.com/"><strong>HTML + JavaScript (jQuery)</strong> – Frontend UI</a></li>
    <li><a href="https://www.pythonanywhere.com/"><strong>PythonAnywhere</strong> – Hosting platform</a></li>
    <li><a href="https://getbootstrap.com/"><strong>Bootstrap</strong> – UI styling</a></li>
    <li><a href="https://globe.gl/"><strong>Globe.gl</strong> – Interactive 3D globe visualization</a></li>
  </ul>

  <h2>Project Structure</h2>
  <pre>
├── server.py            # Flask server that handles API requests
├── countriesDAO.py      # Data Access Object: interfaces with the MySQL database
├── dbconfig.py          # Database credentials and connection info
├── countryviewer.html   # Frontend HTML file for interacting with the service
├── requirements.txt     # List of Python dependencies
└── README.md            # Project documentation
  </pre>

  <h2> Setup Instructions for Running the Page on Your Local Device</h2>
  <h4>1. Clone the Repository</h4>
  <pre><code>git clone &lt;your-repository-url&gt;
cd &lt;project-folder&gt;
</code></pre>

  <h4>2. Install Dependencies</h4>
  <pre><code>pip install -r requirements.txt</code></pre>

  <h4>3. Set Up the Database</h4>
  <p>Create a MySQL database (e.g., on PythonAnywhere) and run the following:</p>
  <pre><code>CREATE TABLE country (
    id INT AUTO_INCREMENT PRIMARY KEY,
    country_name VARCHAR(255),
    visit_date DATE,
    rating INT
);</code></pre>

  <p>Update <code>dbconfig.py</code> with your database credentials:</p>
  <pre><code>mysql = {
    'host': 'your_host',
    'user': 'your_username',
    'password': 'your_password',
    'database': 'your_database_name'
}</code></pre>

  <h4>4. Run the Flask Server (locally)</h4>
  <pre><code>python server.py</code></pre>

  <p>Then visit <code>http://127.0.0.1:5000/countryviewer.html</code> if hosted locally.</p>

  <h2>Live Demo</h2>
  <p>Visit the live version here: 
    <a href="https://aoifeflav.pythonanywhere.com/countryviewer.html" target="_blank">
      https://aoifeflav.pythonanywhere.com/countryviewer.html
    </a>
  </p>

  <h2>Features</h2>
  <ul>
    <li>View all countries with date and rating</li>
    <li>Add a new country</li>
    <li>Update or delete entries</li>
    <li>Displays progress of world coverage as percentage</li>
    <li>Animated rotating 3D globe for visual appeal</li>
  </ul>

  <h2>Sources</h2>
  <ul>
    
  <li>
    <a href="https://www.w3schools.com/html/html_form_input_types.asp" target="_blank">
      W3Schools - HTML Input Types
    </a> – Helped with understanding and using different HTML form input types.
  </li>
  <li>
    <a href="https://chatgpt.com/" target="_blank">
      ChatGPT
    </a> – Used for debugging, code suggestions, improving UI/UX features and writing the README.
  </li>
  <li>
    <a href="https://www.w3schools.com/html/" target="_blank">
      W3Schools - HTML Basics
    </a> – Used to refresh basic HTML syntax and structure.
  </li>
  <li>
    <a href="https://www.w3schools.com/jquery/jquery_ref_ajax.asp" target="_blank">
      W3Schools - jQuery AJAX
    </a> – Helped implement AJAX functionality for frontend-backend communication.
  </li>
  <li>
    <a href="https://blog.pythonanywhere.com/121/" target="_blank">
      PythonAnywhere Blog - Hosting Guide
    </a> – Guided the process of deploying the Flask app online.
  </li>
  <li>
    <a href="https://www.w3schools.com/bootstrap/" target="_blank">
      W3Schools - Bootstrap
    </a> – Helped apply responsive design and styled elements using Bootstrap classes.
  </li>
  <li>
    <a href="https://app.unpkg.com/three@0.77.0" target="_blank">
      unpkg - Three.js
    </a> – Source for the 3D JavaScript library used to visualise the rotating globe.
  </li>
  <li>
    <a href="https://www.w3schools.com/python/python_mysql_getstarted.asp" target="_blank">
      W3Schools - Python & MySQL
    </a> – Helped set up the MySQL database and connector in Python.
  </li>
</ul>

<h4 class="mt-4">Additional Technical Documentation</h4>
<ul>
  <li>
    <a href="https://flask.palletsprojects.com/" target="_blank">
      Flask Documentation
    </a> – Official guide for Flask API usage and routing.
  </li>
  <li>
    <a href="https://www.pythonanywhere.com/" target="_blank">
      PythonAnywhere
    </a> – Platform used for hosting the application.
  </li>
  <li>
    <a href="https://pypi.org/project/mysql-connector-python/" target="_blank">
      MySQL Connector for Python – PyPI
    </a> – Used for database connection and queries.
  </li>
  <li>
    <a href="https://api.jquery.com/" target="_blank">
      jQuery API Reference
    </a> – Consulted for advanced jQuery methods and selectors.
  </li>
  <li>
    <a href="https://github.com/vasturiano/globe.gl" target="_blank">
      Globe.gl Library
    </a> – Library used for rendering the interactive globe in the UI.
  </li>
  <li>
    <a href="https://getbootstrap.com/" target="_blank">
      Bootstrap Official
    </a> – Documentation and components used to build the responsive UI.
  </li>
</ul>

<p><strong>Note:</strong> Course lectures and module-provided materials were also referenced throughout the development of this project.</p>

  </ul>

  <h3>Note</h3>
  <p>This project was originally worked on in my WSAA-coursework folder. Please see that repository here for early stage commit history:</p>
  <li><a href="https://github.com/aoifeflav/WSAA-coursework.git">WSAA-coursework</a></li>
</div>
