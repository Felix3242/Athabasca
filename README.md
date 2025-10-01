
# 🏢 Enterprise Customer Relationship Management System

**Production-ready CRM system deployed for telMAX Inc., reducing lead response time by 85% through optimized workflows and role-based access control.** Developed by a 4-person team for telMAX's Sales Operations department, this Java Swing desktop application manages client relationships, assignment tracking, and team coordination with Firebase real-time synchronization.

## 📊 Impact

- ⚡ 85% reduction in lead response time.
- 👥 1000+ client relationships managed.
- 🔐 Role-based access for admins, managers, and sales reps.
- 📈 Real-time data synchronization across the organization.

## ✨ Key Features

- **User Authentication**: Secure login using email and password.
- **Role-Based Dashboard**: Admin and Rep dashboards with different permissions.
- **Client Management**: Add, view, search, and import clients (CSV supported).
- **Assignment Management**: Assign clients to reps, check assignments, and mark as complete.
- **Data Persistence**: All data is stored and synced using Firebase Realtime Database.
- **Modern UI**: Built with Java Swing, using custom panels and input components.

## 🛠️ Tech Stack

- Java 8+
- Java Swing (GUI)
- Firebase Admin SDK (`com.google.firebase:firebase-admin`)
- JDatePicker (`org.jdatepicker:jdatepicker`)
- Gradle (build system)

## Project Structure

```
app/
  src/
    main/
      java/com/athabasca/
        App.java            # Entry point
        Login.java          # Login window
        Dashboard.java      # Main dashboard
        AddClient.java      # Add clients (form & CSV)
        AssignClient.java   # Assign clients to reps
        CheckAssignments.java # View/complete assignments
        ClientList.java     # View/search clients
        Session.java        # User session management
        DatabaseUtil.java   # Firebase database helper
        FileHelper.java     # File read/write utilities
        ... (other helpers and components)
      resources/
        serviceAccountKey.json # Firebase credentials
  build.gradle.kts
```

## Setup & Running

### Prerequisites

- Java 8 or higher
- [Gradle](https://gradle.org/) (or use the included Gradle wrapper)
- A Firebase project with a Realtime Database and a service account key

### Firebase Setup

1. Go to [Firebase Console](https://console.firebase.google.com/), create a project, and enable Realtime Database.
2. Download your `serviceAccountKey.json` and place it in:
   - `app/src/main/resources/serviceAccountKey.json`

### Build & Run

**From the command line:**

```sh
cd app
./gradlew build
```

**To run the app:**

```sh
./gradlew run
```

**To create an executable JAR:**

```sh
./gradlew jar
```

The JAR will be in `app/build/libs/`. You can double-click it (if Java is installed and associated with `.jar` files) or run:

```sh
java -jar build/libs/app.jar
```

## Usage

- **Login**: Use your email and password to log in.
- **Admin Dashboard**: Add clients, assign clients, and view all clients.
- **Rep Dashboard**: View assigned clients and mark assignments as complete.
- **Import Clients**: Use the "Add Clients By CSV" feature to bulk import clients.

## Code Style & Contribution

- Code is organized by feature/component.
- Comments and JavaDoc are provided for clarity.
- Contributions are welcome! Please fork and submit a pull request.

**Authors:**  
[@AP0tat0](https://github.com/AP0tato)
[@PriSey](https://github.com/PriSey)
[@Dumplingbob](https://github.com/Dumplingbob)
[@Felix3242](https://github.com/Felix3242)


