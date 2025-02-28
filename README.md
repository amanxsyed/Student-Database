# Student Database Management

A simple PostgreSQL-based student database management system that inserts and organizes student, course, and major information from CSV files.

## Features
- Stores student details, including their major and GPA.
- Manages courses and associates them with majors.
- Reads data from CSV files and populates the database.
- Efficiently inserts and updates data using a Bash script.

## Project Structure
```
├── database.sql         # PostgreSQL schema for creating tables
├── insert_data.sh       # Bash script to insert data from CSV files
├── students.csv         # CSV file containing student information
├── courses.csv          # CSV file containing course and major relationships
├── LICENSE              # MIT License
├── README.md            # Project documentation
```

## Prerequisites
- PostgreSQL installed and running
- Bash shell (for executing `insert_data.sh`)
- CSV files (`students.csv`, `courses.csv`) formatted correctly

## Installation & Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/amanxsyed/Student-Database.git
   cd Student-Database
   ```
2. Set up the database:
   ```bash
   psql -U  -d postgres -f database.sql
   ```
3. Load the data:
   ```bash
   ./insert_data.sh
   ```

## Database Schema
The database consists of four tables:
- **students**: Stores student names, major, and GPA.
- **majors**: Stores different majors available.
- **courses**: Stores course details.
- **majors_courses**: Links majors to courses (many-to-many relationship).

## 📞 Connect with Me
- 📧 Email: [amanxsyed@gmail.com](mailto:amanxsyed@gmail.com)
- 💼 LinkedIn: [Syed Aman Shah](https://www.linkedin.com/in/amanxsyed)
- 🐙 GitHub: [@amanxsyed](https://github.com/amanxsyed)

## Contributing

Feel free to fork this repository and submit pull requests for improvements!

## License

This project is licensed under the MIT License.

