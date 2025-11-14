# ToDoCLI 📝

A simple, cross-platform, terminal-based to-do manager written in Rust, backed by SQLite.  
Keep your tasks organized directly from the command line with colored, readable output and persistent storage.

## ✨ Features

- **Lightning Fast**: Built with Rust for maximum performance
- **Persistent Storage**: Uses SQLite database to keep your tasks safe
- **Simple Interface**: Clean and intuitive command-line interface
- **Color-Coded Output**: Visual status indicators for better task management
- **Cross-Platform**: Works on Linux, macOS, and Windows
- **Sort & Filter**: Organize tasks by status or ID
- **Fully Tested**: Comprehensive test suite ensuring reliability

## 📦 Installation

### Prerequisites

- Rust 1.70 or higher
- Cargo (comes with Rust)

### Build from Source

```bash
# Clone the repository
git clone https://github.com/CanReader/todocli.git
cd todocli

# Build the project
cargo build --release

# The binary will be available at target/release/todo
```

### Install Globally

```bash
cargo install --path .
```

## 🚀 Usage

### Basic Commands

#### Add a Task
```bash
todo add "Buy groceries"
todo add "Finish project documentation"
```

#### List All Tasks
```bash
todo list
```

#### Toggle Task Status
```bash
todo toggle 1
```

#### Remove a Task
```bash
todo rm 3
```

#### Sort Tasks by Status
```bash
todo sort
```

#### Reset Database
```bash
todo reset
```
*Note: This command will ask for confirmation before deleting all tasks.*

#### Show Help
```bash
todo help
```

## 📋 Command Reference

| Command | Description | Example |
|---------|-------------|---------|
| `add [TASK]` | Add a new task | `todo add "Write documentation"` |
| `list` | Display all tasks sorted by ID | `todo list` |
| `toggle [ID]` | Toggle task status (Done/Pending) | `todo toggle 2` |
| `rm [ID]` | Remove a specific task | `todo rm 5` |
| `sort` | Display tasks sorted by status | `todo sort` |
| `reset` | Delete all tasks (with confirmation) | `todo reset` |
| `help` | Show available commands | `todo help` |

## 🎨 Output Example

```
TODO List (sorted by id):
   1 | Buy groceries                                Pending  2024-01-15 10:30:00
   2 | Finish project documentation                 Done     2024-01-15 11:45:00
   3 | Call dentist                                 Pending  2024-01-15 14:20:00
```

## 🗄️ Database Location

ToDoCLI stores its database in your home directory:

- **Linux/macOS**: `~/todo_db/todo.sqlite`
- **Windows**: `%USERPROFILE%\todo_db\todo.sqlite`

The database and directory are created automatically on first use.

## 🛠️ Technologies Used

- **Rust**: Core programming language
- **rusqlite**: SQLite database interface
- **console**: Terminal styling and colors
- **dialoguer**: Interactive CLI prompts
- **lazy_static**: Static initialization for tests

## 🧪 Running Tests

```bash
cargo test
```

The project includes comprehensive unit tests covering:
- Adding tasks
- Listing tasks
- Toggling task status
- Removing tasks
- Sorting tasks
- Database reset functionality

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🌟 Acknowledgments

- Built with ❤️ using Rust
- Inspired by the need for a simple, fast task manager

---

**Happy Task Managing! 📝✅**

