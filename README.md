# BinCrack

**BinCrack** is a gamified learning platform for binary exploitation, designed to provide hands-on experience and enhance cybersecurity skills through interactive challenges. Built using C++ and MySQL, the project offers a structured and engaging environment for students, enthusiasts, and CTF competitors. This project is part of my **Workshop 1** subject.

---

## Features

- **User Management**
  - Secure user registration and login with hashed passwords.
  - Account deletion for personal data management.

- **Challenge Management**
  - Challenges categorized into `Easy`, `Medium`, and `Hard` levels.
  - Dynamic scoring system based on challenge difficulty.
  - Hint system with penalty deduction.

- **Gamification**
  - Leaderboard showcasing top players.
  - Badge awarding system for achievements.

- **Educational Focus**
  - Interactive gameplay to enhance cybersecurity skills.
  - Focus on binary exploitation challenges.

---

## Project Setup

### Prerequisites

1. **Development Environment**
   - Windows with Visual Studio 2022 or similar IDE.
   - MySQL Server installed and running.
   - MySQL C++ Connector.

2. **Database Configuration**
   - Create a MySQL database named `bincrack_db`.
   - Execute the provided SQL script (`bincrack_schema.sql`) to create necessary tables.

### Installation Steps

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/BinCrack.git
   ```

2. Open the project in your IDE.

3. Configure the database credentials in the `main()` function:
   ```cpp
   const string server = "tcp://127.0.0.1:3306";
   const string username = "your_username";
   const string password = "your_password";
   const string database = "bincrack_db";
   ```

4. Build and run the project.

---

## Usage

1. **Start the Program**
   - The program launches with a main menu offering options to register, login, or exit.

2. **Player Dashboard**
   - Once logged in, users can access challenges, view leaderboards, and earned badges.

3. **Challenge System**
   - Attempt challenges by providing correct solutions.
   - Use hints if necessary (with penalty).

4. **Gamified Progression**
   - Earn points and badges to climb the leaderboard.
   - Track completed challenges.

---

## File Structure

```
BinCrack/
├── src/                    # Source files
│   ├── main.cpp            # Entry point
│   ├── BadgeManager.h      # Badge-related logic
│   └── utils/              # Utility functions
├── db/                     # Database scripts
│   └── bincrack_schema.sql # Database schema setup
├── README.md               # Project documentation
└── LICENSE                 # License file
```

---

## Database Schema

### Tables

1. **Players**
   - Stores user information such as username, hashed password, score, and last login.

2. **Challenges**
   - Contains challenges with details like name, difficulty, description, solution, and hints.

3. **Challenge_Completion**
   - Tracks challenges completed by players, including timestamps.

4. **Badges**
   - Stores badge details like name, description, and awarding criteria.

5. **Awarded_Badges**
   - Tracks badges awarded to players with timestamps.

---

## Future Improvements

- Add an admin panel for managing challenges and badges.
- Transition to a GUI for better user experience.
- Introduce dynamic challenge generation.
- Enhance security with two-factor authentication and stronger hashing algorithms.
- Enable multi-user real-time interaction.

---

## Contributing

Contributions are welcome! Please fork the repository, make your changes, and submit a pull request.

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## Contact

For any inquiries or suggestions, please contact [your-email@example.com].
