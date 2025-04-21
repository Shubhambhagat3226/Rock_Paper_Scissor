# Rock Paper Scissor - Java Swing Game

A classic Rock Paper Scissor game implemented in Java with a simple Swing GUI. Play against the computer and track your score!


## Table of Contents

*   [Features](#features)
*   [Technologies Used](#technologies-used)
*   [Prerequisites](#prerequisites)
*   [Getting Started](#getting-started)
    *   [Option 1: Running from the Command Line](#option-1-running-from-the-command-line)
    *   [Option 2: Running from an IDE (IntelliJ, Eclipse, etc.)](#option-2-running-from-an-ide-intellij-eclipse-etc)
    *   [Option 3: Creating and Running an Executable JAR (Advanced)](#option-3-creating-and-running-an-executable-jar-advanced)
*   [How to Play](#how-to-play)
*   [Project Structure](#project-structure)
*   [Contributing](#contributing)

## Features

*   Simple and intuitive graphical user interface (GUI) built with Java Swing.
*   Classic Rock Paper Scissor gameplay against the computer.
*   Random computer choice for each round.
*   Score tracking for both player and computer.
*   Clear display of computer's choice and round result.
*   Easy "Try Again" button for quick restarts.

## Technologies Used

*   **Java:** The core programming language.  Requires JDK version 8 or later.
*   **Swing:**  The Java GUI toolkit used for the user interface.  (Part of the standard Java library.)

## Prerequisites

*   **Java Development Kit (JDK)**:  You must have the JDK installed.  Download from [Oracle](https://www.oracle.com/java/technologies/javase-downloads.html) or an open-source distribution like [AdoptOpenJDK](https://adoptopenjdk.net/). Verify your installation by opening a terminal or command prompt and running:

    ```bash
    java -version
    javac -version
    ```

    You should see version information for both `java` and `javac`.

## Getting Started

Choose one of the following methods to run the game:

### Option 1: Running from the Command Line

This is the simplest way to run the game if you are comfortable with the command line.

1.  **Download the Source Code:** Clone the repository (if available) or download the ZIP file containing the source code and extract it to a directory on your computer.

2.  **Navigate to the Project Directory:** Open a terminal or command prompt and change the directory to the root of the project (the directory containing the `src` folder).

    ```bash
    cd path/to/shubhambhagat3226-rock_paper_scissor
    ```

3.  **Compile the Java Code:** Compile all the `.java` files in the `src` directory:

    ```bash
    javac src/*.java
    ```

    This creates `.class` files in the `src` directory. If you get errors, double-check that you have the JDK installed correctly and that `javac` is in your system's PATH.

4.  **Run the Application:** Execute the `App` class:

    ```bash
    java -cp src App
    ```

    *   `-cp src` tells Java where to find the compiled `.class` files (in the `src` directory).
    *   `App` is the name of the main class (the one with the `main` method).

### Option 2: Running from an IDE (IntelliJ, Eclipse, etc.)

Using an IDE simplifies the process of compiling and running Java code.

1.  **Open your IDE:** Launch your preferred Java IDE (e.g., IntelliJ IDEA, Eclipse, NetBeans, VS Code with Java extensions).

2.  **Import the Project:**
    *   **IntelliJ IDEA:**  "Open" and select the `shubhambhagat3226-rock_paper_scissor` directory.  IntelliJ should automatically recognize it as a Java project (if the `.iml` file is present)
    *   **Eclipse:** "Import" -> "Existing Projects into Workspace" and select the project directory.

3.  **Run the `App` Class:**  Locate the `src/App.java` file in the project explorer. Right-click on it and select "Run" or "Run As -> Java Application".

### Option 3: Creating and Running an Executable JAR (Advanced)

This option creates a single `.jar` file that you can run without needing to compile the code every time.

1.  **Compile the Code:** (If you haven't already):

    ```bash
    javac src/*.java
    ```

2.  **Create the JAR File:**  Navigate to the project root directory and execute the following command:

    ```bash
    jar cvfm RockPaperScissor.jar src/META-INF/MANIFEST.MF -C src .
    ```

    *   `jar`: The Java archive tool.
    *   `cvfm`: Options: `c` (create), `v` (verbose), `f` (file name), `m` (manifest file).
    *   `RockPaperScissor.jar`: The name of the JAR file to create.
    *   `src/META-INF/MANIFEST.MF`:  The path to the manifest file, which tells Java which class is the entry point (`App`).
    *   `-C src .`: Change to the `src` directory and include all files in the current directory (`.`) in the JAR.

3.  **Run the JAR File:**

    ```bash
    java -jar RockPaperScissor.jar
    ```

## How to Play

1.  Launch the application.
2.  Click "Rock", "Paper", or "Scissor" to make your move.
3.  The computer's choice will be displayed.
4.  The game result ("Player Wins", "Computer Wins", or "Draw") will be shown.
5.  The scores will be updated.
6.  Click the "Try Again?" button to play another round.

## Project Structure

```
Directory structure:
└── shubhambhagat3226-rock_paper_scissor/
    ├── Rock Paper Scissor Game.iml
    └── src/
        ├── App.java
        ├── RockPaperScissor.java
        ├── RockPaperScissorGUI.java
        └── META-INF/
            └── MANIFEST.MF
```

## Contributing

If you'd like to contribute, feel free to fork the repository and submit a pull request with your changes.  Please follow these guidelines:

*   Use clear and descriptive commit messages.
*   Write clean and well-documented code.
*   Test your changes thoroughly.
