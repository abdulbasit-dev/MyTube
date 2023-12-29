# MyTube: Video Processing System

MyTube is a straightforward Java project designed to simulate a video processing system. <br> Below is an organized overview of the project, including its structure and key classes.

## Project Structure

```
MyTube/
├── .gitignore
├── .idea/
├── MyTube.iml
├── README.md
└── src/
    └── com/
        └── mytube/
            ├── EmailService.java
            ├── Main.java
            ├── NotificationService.java
            ├── SqlVideoDatabase.java
            ├── User.java
            ├── Video.java
            ├── VideoDatabase.java
            ├── VideoEncoder.java
            ├── VideoProcessor.java
            └── XVideoEncoder.java
```

## Classes

### `EmailService`
- Responsible for sending email notifications.
- Implements the `NotificationService` interface.

### `Main`
- Entry point of the application.
- Creates a `Video` object, sets its properties, and processes it using a `VideoProcessor`.

### `NotificationService`
- Interface for services that send notifications.

### `SqlVideoDatabase`
- Manages the storage of video metadata.
- Implements the `VideoDatabase` interface.

### `User`
- Represents a user in the system.

### `Video`
- Represents a video in the system.
- Properties include the file name, title, and user.

### `VideoDatabase`
- Interface for databases that store video metadata.

### `VideoEncoder`
- Interface for services that encode videos.

### `VideoProcessor`
- Processes videos using a `VideoEncoder`, `VideoDatabase`, and `NotificationService`.
- Responsible for encoding the video, storing its metadata, and notifying the user.

### `XVideoEncoder`
- Encodes videos and implements the `VideoEncoder` interface.

## How to Run

To run the project, execute the `Main` class.