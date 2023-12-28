# internsctl(1) - Custom Linux Command

## NAME

internsctl - Custom Linux command for various operations

## SYNOPSIS

**internsctl** [options] [command] [arguments]

## DESCRIPTION

`internsctl` is a custom Linux command that provides various functionalities for system management.

## OPTIONS

- `--help`: Show help information.
- `--version`: Show command version.

## COMMANDS

- `cpu`: Perform operations related to CPU.
  - `getinfo`: Get information about the CPU.

- `memory`: Perform operations related to memory.
  - `getinfo`: Get information about memory.

- `user`: Manage user accounts.
  - `create <username>`: Create a new user.
  - `list [--sudo-only]`: List all regular users or users with sudo permissions.

- `file`: Perform operations related to files.
  - `getinfo <file-name>`: Get information about a file.

## EXAMPLES

- Create a new user:
  ```bash
  internsctl user create john

