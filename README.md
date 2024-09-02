# Project_porfolio
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Samiksha Gupta | Data Science Student</title>
  <link rel="stylesheet" href="styles.css">
  <style>
    /* ... (same CSS as before) ... */

    /* New styles */
    body {
      background-color: #f5f5f5;
    }

    header {
      background-size: cover;
      background-position: center;
      color: #fff;
    }

    section {
      background-color: #fff;
      padding: 2rem;
      border-radius: 10px;
      box-shadow: 0px 2px 4px rgba(0, 0, 0, 0.1);
    }

    .project-card {
      display: flex;
      align-items: center;
      padding: 1rem;
      border-bottom: 1px solid #ddd;
    }

    .project-card img {
      width: 100px;
      height: 100px;
      object-fit: cover;
      margin-right: 1rem;
    }

    .project-card h4 {
      margin-bottom: 0;
    }
  </style>
</head>

<body>
  <header>
    <h1>Samiksha Gupta</h1>
    <nav>
      <ul>
        <li><a href="#about">About</a></li>
        <li><a href="#projects">Projects</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <main>
    <section id="about">
      <h2>About Me</h2>
      <p>Hello! I am Samiksha Gupta. I am a student at Christ University, Pune, Lavasa. I am pursuing Bsc in Data Science.</p>
    </section>

    <section id="skills">
      <h2>Skills</h2>
      <ul>
        <li>HTML5 & CSS3</li>
        <li>Python</li>
        <li>R programming</li>
        <li>Canva</li>
        <li>Advanced Excel</li>
      </ul>
    </section>

    <section id="projects">
      <h3>Projects</h3>
      <div class="project-card">
        <img src="project_1.png" alt="Project 1">
        <h4>Project One - Hotel Management System in Python</h4>
        <a href="project_1.html">View Project</a>
      </div>
      <div class="project-card">
        <img src="project_2.png" alt="Project 2">
        <h4>Project Two -  Exploratorary Data Analyasis</h4>
	<a href="project_2.html">View Project</a>
       </div>
    </section>

    <section id="contact">
      <h2>Contact</h2>
      <p>Email: samikshagupta2719@gmail.com</p>
    </section>
  </main>

  <footer>
    <p>&copy; 2024 Samiksha Gupta. All rights reserved.</p>
  </footer>
</body>

</html>
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Hotel Management System</title>
  <link rel="stylesheet" href="styles.css"> </head>
<body>
  <header>
    <h1>Hotel Management System</h1>
  </header>

  <main>
    <section>
      <h2>Overview</h2>
      <p>This project is a Python-based application that allows users to manage hotel guest information.</p>
      <ul>
        <li>Insert new guest records</li>
        <li>Update existing guest information</li>
        <li>Delete guest records</li>
        <li>Display all the guest records</li>
      </ul>
    </section>

    <section>
      <h2>Features</h2>
      <ul>
        <li>Efficient data management</li>
        <li>Secure authentication</li>
      </ul>
    </section>

    <section>
      <h2>Screenshots</h2>
      <img src="project_1.png" alt="Screenshot 1">
      </section>

    <section>
      <h2>Code Sample</h2>
      <pre>
        <code>
def update_guest(U,room_no, new_name=None, new_room_no=None, new_people=None, new_type_room=None):
    try:
        guest_details = U[room_no] 
        if new_name:
            guest_details['Name'] = new_name
        if new_room_no:
            guest_details['Room No.'] = new_room_no
        if new_people:
            guest_details['No. of people'] = new_people
        if new_type_room:
            guest_details['Type of room Alloted'] = new_type_room
        print("Guest details updated successfully!")
        
    except KeyError:
        print("Invalid Room Number.") 
        
         </code>
      </pre>
    </section>
  </main>

  <footer>
    <p>&copy; 2024 Samiksha Gupta. All rights reserved.</p>
  </footer>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Exploratory Data Analysis</title>
  <link rel="stylesheet" href="styles.css"> </head>
<body>
  <header>
    <h1>Exploratory Data Analysis</h1>
  </header>

  <main>
    <section>
      <h2>Overview</h2>
      <p>This project is a Python-based group project that </p>
      <ul>
        <li>Data Collection</li>
        <li>Data Cleaning</li>
        <li>Data Visualization</li>
        <li>Identify Patterns and Outliers</li>
      </ul>
    </section>

    <section>
      <h2>Features</h2>
      <ul>
        <li>Finding insights</li>
        <li>Graphical Analysis</li>
      </ul>
    </section>

    <section>
      <h2>Screenshots</h2>
      <img src="project_2.png" alt="Screenshot 1">
      <img src="project_2(1).png" alt="Screenshot 2">
      </section>

    <section>
      <h2>Code Sample</h2>
      <pre>
        <code>
player_goals = df2.groupby('Name')['goals scored '].sum().reset_index().sort_values(by='goals scored ', ascending=False)
plt.figure(figsize=(10, 6))
sns.barplot(data=player_goals.head(10), x='goals scored ', y='Name', palette='Blues_r')
plt.xlabel('Total Goals Scored')
plt.ylabel('Player Name')
plt.title('Top Scorers')
plt.show() 
        
         </code>
      </pre>
    </section>
  </main>

  <footer>
    <p>&copy; 2024 Samiksha Gupta. All rights reserved.</p>
  </footer>
</body>
</html>
body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
    margin: 0;
    padding: 0;
    color: #333;
}

header {
    background-color: #2970e3;
    color: #fff;
    padding: 10px 0;
    text-align: center;
}

nav ul {
    list-style: none;
    padding: 0;
}

nav ul li {
    display: inline;
    margin: 0 15px;
}

nav ul li a {
    color: #fff;
    text-decoration: none;
}

main {
    padding: 20px;
}

section {
    margin-bottom: 20px;
}

h2 {
    border-bottom: 2px solid #444;
    padding-bottom: 5px;
}

footer {
    background-color: #2970e3;
    color: #fff;
    text-align: center;
    padding: 10px 0;
    position: fixed;
    bottom: 0;
    width: 100%;
}

@media (max-width: 600px) {
    nav ul li {
        display: block;
        margin: 10px 0;
    }
}
