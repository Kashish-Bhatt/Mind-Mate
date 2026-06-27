# MindMate

A Java Desktop Application for Mental Wellness Tracking

## 📌 Overview

MindMate is a desktop application built in Java that helps users track their mental wellness through daily mood logging, habit tracking, and an integrated chatbot for support and interaction. The app provides visual insights through charts to help users understand patterns in their mood and habits over time.

Built using Java Swing for the GUI and SQLite for persistent data storage, MindMate combines multiple features — authentication, tracking, analytics, and chat — into a single standalone desktop application.

## 🎯 Objectives

- Provide a simple way for users to track their daily mood
- Help users build and maintain daily habits
- Offer visual insights (charts/graphs) based on user activity
- Provide an integrated chatbot for mental health support and interaction
- Build a complete, multi-feature desktop application using core Java OOP principles

## 🧠 Technologies Used

- Java (Core + OOP)
- Java Swing (GUI)
- SQLite (database)
- JDBC (database connectivity)

## ✨ Core Features

### 🔐 User Authentication
- User Sign Up and Login
- Separate handling for regular users and admin (AdminFrame)
- Credential validation

### 🏠 Home Dashboard
- Central landing page after login (HomePanel)
- Navigation to all major features
- Quick overview/shortcuts

### 📊 Mood Tracking
- Log daily mood entries (MoodTrackerPanel)
- Store and manage mood history
- View past mood data

### 🎯 Habit Tracker
- Add and manage daily habits (HabitTrackerPanel)
- Track consistency and progress over time

### 📈 Insights & Analytics
- Visual insights dashboard (InsightsPanel)
- Pie charts and bar graphs based on mood/habit data
- Data-driven feedback on user activity

### 🤖 Chatbot
- Integrated chatbot (ChatbotPanel)
- Provides conversational mental health support and interaction

### 🧭 Sidebar Navigation
- Dedicated sidebar (SidebarPanel) for switching between:
  - Home
  - Mood Tracker
  - Habit Tracker
  - Insights
  - Chatbot

### 💾 Database Integration
- Uses SQLite (mindmate.db) for persistent storage
- Managed through DatabaseHelper
- Stores user data, mood entries, and habits
- Initial data setup handled via SeedData.java

### 👤 User Management
- User.java defines the user model
- UserFrame for user-specific UI
- AdminFrame for admin-level controls

### 🎨 UI/UX Design
- Custom theming via AppTheme for consistent styling across the app
- Built entirely with Java Swing

### ⚡ Splash Screen
- Custom startup splash screen (SplashScreen) for a polished launch experience

### 📦 Standalone Packaging
- Exported as a runnable JAR (MindMate.jar)
- Includes manifest.txt for execution configuration

## 📁 Project Structure

MindMate/
├── src/ (Java source code)
│ ├── HomePanel.java
│ ├── MoodTrackerPanel.java
│ ├── HabitTrackerPanel.java
│ ├── InsightsPanel.java
│ ├── ChatbotPanel.java
│ ├── SidebarPanel.java
│ ├── User.java
│ ├── UserFrame.java
│ ├── AdminFrame.java
│ ├── DatabaseHelper.java
│ ├── SeedData.java
│ ├── AppTheme.java
│ ├── SplashScreen.java
│ └── ...
├── lib/ (External libraries/JARs)
├── mindmate.db (SQLite database)
└── README.md

## 🚀 How to Run

1. Clone the repository

git clone https://github.com/Kashish-Bhatt/MindMate.git

2. Open the project in your preferred Java IDE (IntelliJ IDEA, Eclipse, or VS Code with Java extensions)

3. Make sure the SQLite JDBC driver (in lib/) is added to your project's build path/classpath

4. Run the main class to launch the application

5. Sign up for a new account or log in to start tracking your mood and habits

## 🔮 Future Improvements

- Add data export (e.g. PDF/CSV reports of mood and habit history)
- Improve chatbot responses with a more advanced NLP model
- Add notifications/reminders for habit tracking
- Migrate UI from Swing to a modern framework (e.g. JavaFX)
