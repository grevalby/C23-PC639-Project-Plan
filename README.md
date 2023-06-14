### How to run this project on your local machine

_This project uses Laravel as the framework, before you can run tanitama-backend project in your local machine, you should ensure that your local machine has **PHP** and **Composer** installed._

**1. Clone the repo**
- Open your terminal or command prompt.
- Navigate to the directory where you want to store the project.
- Use the git clone command followed by the repository's URL. For example:
   ```bash
   git clone https://github.com/grevalby/tanitama-backend.git
   ```

**2. Install Dependencies**
- Navigate to the project's directory
   ```bash
   cd tanitama-backend
   ```
- Once inside the project's directory, use a package manager like Composer to install the project's dependencies. Run the following command:
  ```sh
  composer install
  ```
  This command will download and install all the required PHP packages specified in the project's **'composer.json'** file.

**3. Create the Environment File**
- Laravel requires an environment file to store configuration settings.
- Copy the **'.env.example'** file in the project's root directory and rename it to **'.env'** :
   ```bash
   cp .env.example .env
   ```
- Customize the settings in the **'.env'** file, such as the database connection details.

**4. Generate an Application Key**
- The Laravel framework uses an application key for encryption and other security purposes.
- Generate an application key using the **'artisan'** command:
  ```vbnet
   php artisan key:generate
  ```

**5. Run Database Migrations**
- Laravel uses migrations to manage the database schema.
- Run the following command to execute the migrations and create the necessary tables in the database:
  ```sh
    php artisan migrate
  ```

**6. Serve the Application**
- You can use Laravel's built-in development server to run the application locally.
- Start the server by running the following command:
  ```sh
    php artisan serve
  ```
- The application should now be running at http://localhost:8000 by default.

  
