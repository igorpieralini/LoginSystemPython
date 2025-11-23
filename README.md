# 🔒 LoginPage - Python Login System

This project implements a login page using Python with the **Tkinter** library and a **MariaDB/MySQL** database connection. The goal is to authenticate users using a graphical form, providing a simple and effective login for desktop systems. After a successful login, the system redirects the user to the registration page.

## ⚙️ Features

* 🔐 User authentication via a graphical form (GUI) with email and password.
* 🔗 Connection to MariaDB/MySQL database for user validation.
* ⚠️ Error handling, such as database connection failure or invalid credentials.
* ➡️ Redirect to the registration page after a successful login.

## 📂 Project Structure

* **LoginForm**: Class responsible for the login GUI, handling events, and user authentication.
* **CadastroForm**: Class responsible for the registration GUI and database connection to store user data.

## 🛠️ Requirements

* 🐍 **Python 3.8+**
* 🐬 **MariaDB/MySQL**
* 📦 **Required Python libraries**:

  * `mysql-connector-python`
  * `tkinter` (included in standard Python)

You can install the MySQL connector using the following command:

```bash
pip install mysql-connector-python
```

## ⚙️ Database Setup

1. 🖥️ Start the MariaDB/MySQL server using XAMPP or another tool.
2. 📊 Create a database called `pieralini__login`.
3. 📝 Create a `users` table with the following fields:

   ```sql
   CREATE TABLE users (
       id INT AUTO_INCREMENT PRIMARY KEY,
       name VARCHAR(100),
       email VARCHAR(100) UNIQUE,
       phone VARCHAR(15),
       address VARCHAR(255),
       password VARCHAR(100)
   );
   ```
4. ➕ Insert some test records to validate the login system.

## ▶️ How to Run

1. 💻 Make sure Python 3 is installed on your system.
2. ⚙️ Configure the database according to the instructions above.
3. 🐍 Run the Python script to start the application:

   ```bash
   python login_form.py
   ```

## 📞 Contact

* **Developer**: Igor Pieralini
* ✉️ **Email**: [igorpieralini@gmail.com](mailto:igorpieralini@gmail.com)

Feel free to reach out with questions or suggestions!

## 🌟 Future Improvements

* 🔒 Implement password hashing for increased security.
* ➕ Add password recovery options.
* 🎨 Improve the GUI for a more friendly and responsive interface.
