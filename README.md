# College Connect - Student Networking & Event Discovery Platform

## Overview

College Connect is a Java-based console application that enables students to build academic and professional connections within their college community. The platform combines social networking, friend recommendations, note sharing, and personalized event discovery into a single system.

Users can create profiles, connect with peers, discover students with similar interests, share notes with friends, and receive event recommendations tailored to their interests. Administrators can manage events and maintain event listings for different colleges.

---

## Features

### User Management
- User registration and login authentication
- Profile creation and editing
- Personal information, bio, interests, and professional details management
- Input validation and exception handling

### Student Networking
- Send and receive connection requests
- Accept, decline, or withdraw requests
- View and manage friend lists
- Remove existing connections

### Friend Recommendation System
- Recommendations based on mutual connections
- Recommendations based on common interests
- Priority ranking using a custom Max Heap implementation
- Displays the most relevant potential connections

### User Search
- Search users by name
- Search users by interests
- View mutual friends and matching interests

### Notes Sharing
- Create and update personal notes
- View notes shared by friends

### Event Management

#### Admin Features
- Add new events
- Edit event details
- Mark events as completed
- View all events

#### User Features
- View events by date
- View events within a selected date range
- Receive personalized event recommendations
- Search events using keywords

### Personalized Event Recommendations
- Matches user interests with event keywords
- Sorts events based on relevance
- Supports additional keyword-based filtering

### File-Based Data Persistence
Stores and retrieves:
- User profiles
- Friend connections
- Connection requests
- User notes
- Event records

---

## Technologies Used

- Java
- Object-Oriented Programming (OOP)
- Java Collections Framework
  - HashMap
  - HashSet
  - ArrayList
- Custom Max Heap
- File Handling
- Exception Handling
- LocalDate API

---

## System Architecture

| Class | Responsibility |
|---------|---------------|
| User | User profile management and networking operations |
| FileHandler | File storage and retrieval operations |
| Recommendation | Stores recommendation details |
| MaxHeap | Prioritizes recommendation results |
| Event | Stores event information |
| eventDisplay | Event filtering and recommendation logic |
| Admin | Event administration |
| Main | Application entry point |

---

## Recommendation Engine

### Friend Recommendations
The platform recommends users based on:
- Number of mutual friends
- Number of common interests

A custom Max Heap data structure is used to rank recommendations and display the most relevant users first.

### Event Recommendations
The platform recommends events by:
- Matching user interests with event keywords
- Filtering events belonging to the user's college
- Ranking events based on keyword relevance

---

## Project Structure

```text
profile.txt      -> User profile data
friends.txt      -> Friend connections
requests.txt     -> Pending connection requests
notes.txt        -> User notes
events.txt       -> Event information
```

---

## How to Run

### Prerequisites
- Java JDK 8 or above
- Any Java IDE (IntelliJ IDEA, Eclipse, VS Code) or terminal

### Compile

```bash
javac Main.java
```

### Run

```bash
java Main
```

---

## Application Workflow

### User Side
1. Register and create a profile
2. Login to the platform
3. Add interests and profile details
4. Discover students through recommendations
5. Send and manage connection requests
6. View friends and shared notes
7. Explore personalized event recommendations

### Admin Side
1. Login using admin credentials
2. Add and manage events
3. Update event information
4. Mark events as completed
5. Monitor event listings

---

## Concepts Demonstrated

- Object-Oriented Programming
- Data Structures & Algorithms
- Priority Queues (Max Heap)
- Recommendation Systems
- Searching & Filtering
- File-Based Data Management
- Exception Handling
- Modular Software Design

---

## Future Enhancements

- GUI using JavaFX or Swing
- Database integration (MySQL/PostgreSQL)
- Password encryption
- Real-time messaging system
- Event registration functionality
- Notification system
- Web and mobile application versions

---

## Authors

Developed as a Java-based academic project to explore networking systems, recommendation algorithms, event management, and file-based data persistence.
