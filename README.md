Certainly! Here's a consolidated version of the README with the entire content, including usage examples:

```markdown
# internsctl

**Custom Linux Command for System Management**

![internsctl Logo](path/to/your/logo.png)

## Introduction

`internsctl` is a custom Linux command designed to streamline various system management tasks. It provides a set of functionalities related to CPU, memory, user management, and file operations.

## Features

- **CPU Operations:**
  - Get CPU information.

- **Memory Operations:**
  - Get memory information.

- **User Operations:**
  - Create a new user.
  - List all regular users.
  - List users with sudo permissions.

- **File Operations:**
  - Get information about a file.

## Installation

Clone the repository to your local machine:

```bash
git clone https://github.com/yourusername/internsctl.git
```

Move the `internsctl` script to a directory in your `$PATH` for global access:

```bash
sudo mv internsctl/scripts/internsctl /usr/local/bin/
```

Move the man page (`internsctl.1`) to the man page directory:

```bash
sudo mv internsctl/docs/internsctl.1 /usr/share/man/man1/
```

Update the man database:

```bash
sudo mandb
```

## Usage

```bash
internsctl [options] [command] [arguments]
```

## Command Options

- `--help`: Show help information.
- `--version`: Show command version.

### CPU Operations:

- `cpu getinfo`: Get information about the CPU.

### Memory Operations:

- `memory getinfo`: Get information about memory.

### User Operations:

- `user create <username>`: Create a new user.
- `user list [--sudo-only]`: List all regular users or users with sudo permissions.

### File Operations:

- `file getinfo <file-name>`: Get information about a file.

## Examples

- Create a new user:

  ```bash
  internsctl user create john
  ```

- List all regular users:

  ```bash
  internsctl user list
  ```

- List users with sudo permissions:

  ```bash
  internsctl user list --sudo-only
  ```

- Get information about a file:

  ```bash
  internsctl file getinfo /path/to/file
  ```

## Documentation

Detailed documentation is available in the [Manual Page](docs/internsctl-manual.md).

## Folder Structure

```
internsctl/
|-- scripts/
|   |-- internsctl             # Bash script for the internsctl command
|-- docs/
|   |-- internsctl-manual.md   # Manual documentation in Markdown format
|   |-- internsctl.1           # Generated man page
|-- .gitignore                 # Gitignore file to exclude unnecessary files
|-- README.md                  # Project README with instructions and information
|-- CONTRIBUTING.md            # Guidelines for contributing to the project
|-- LICENSE                    # License information
```

## Diagrams

- [Workflow Diagram](diagrams/workflow-diagram.png): Provides a visual representation of the command workflow.
- [Architecture Diagram](diagrams/architecture-diagram.png): Illustrates the application architecture.


