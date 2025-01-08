YouTube Music Launcher 

This Go application listens for keyboard events and triggers an action when a specific key is pressed. It leverages the go-hook package to monitor low-level keyboard events and executes a command to open YouTube Music in a private Firefox window when the . (dot) key is pressed.
Features

    Keyboard Monitoring: Continuously listens for global keyboard events on the system.
    Custom Actions: Detects when the . key is pressed and launches YouTube Music in a private Firefox browser window.
    Interrupt Handling: Gracefully handles system interrupts (e.g., Ctrl+C) to clean up resources.

Prerequisites

    Operating System: Windows (required for cmd commands and go-hook functionality).
    Browser: Firefox must be installed on the system.

Dependencies

    moutend/go-hook: Provides the ability to hook into keyboard events.

Installation

    Clone the repository:

git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name

Install dependencies:

go mod tidy

Build and run the application:

    go build
    ./your-app-name

Example Usage

    Run the application:

    ./your-app-name

    Press the . key on your keyboard.
    Firefox will open YouTube Music in a private browsing window.

Notes

    Ensure that the application has appropriate permissions to hook into system-level keyboard events.
    Modify the exec.Command function if you want to use a different browser or command.
