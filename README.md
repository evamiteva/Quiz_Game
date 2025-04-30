# Quiz_Game

# Features
- Real-time multiplayer using SignalR.

- Players can join the game by entering their name.

- Questions are broadcasted to all players simultaneously.

- Players can submit answers, which are shared across all participants.

- Supports multiple players playing the quiz simultaneously.

# Getting Started
These instructions will help you set up and run the project locally.

# Prerequisites
.NET 8 SDK installed (or higher).

Visual Studio 2022 or another IDE with .NET support.

A web browser (Chrome, Firefox, Edge, etc.).

# Installation
Clone the repository

Open the project in Visual Studio 2022.

Restore NuGet packages:

In Visual Studio, right-click on the solution and select Restore NuGet Packages.

Install SignalR:

Right-click on the project → Manage NuGet Packages → Search for Microsoft.AspNetCore.SignalR and install it.

Set the project as StartUp Project if it isn't already.

Run the project by pressing F5 or clicking Start Debugging.

# Running the Application
Once the project is running, you can access the game at:

https://localhost:<port>/Game

You can open this URL in multiple browser tabs to test the multiplayer functionality.

# How It Works
Joining the Game: Players type their name and click "Join Game".

Receiving Questions: A quiz question will be sent to all connected players once the game starts.

Answering the Question: Players can submit their answers, which will be displayed to everyone in real-time.

SignalR Hub: The QuizHub class in Hubs/QuizHub.cs handles communication between the server and clients.

# Customization
Questions: To add more questions, modify the SendQuestion method in the QuizHub.cs class.

Game Logic: You can add features such as score tracking, timers, and more.
