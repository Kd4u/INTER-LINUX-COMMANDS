<img width="431" alt="Screenshot 2023-11-02 at 7 29 21 PM" src="https://github.com/Kd4u/INTER-LINUX-COMMANDS/assets/96914340/6952e427-e543-437c-9a00-168f74ba5a98"># INTER-LINUX-COMMANDS
INTERN LINUX COMMANDS CREATION
STEPS INVOLVED IN THE PROBLEM

Here's all elements explanation of the code:

#!/bin/bash: This is called a shebang and specifies the interpreter to be used to execute the script, in this case, it is Bash.
VERSION="v0.1.0": This line defines a variable VERSION and assigns it the value "v0.1.0". This variable is used to store the version number of the script.

function display_help() { ... }: This defines a function named display_help that displays the usage information and available options when called.

get_cpu_info() { ... }: This defines a function named get_cpu_info that retrieves and displays CPU information from the /proc/cpuinfo file.
get_memory_info() { ... }: This defines a function named get_memory_info that retrieves and displays memory information from the /proc/meminfo file.

create_user() { ... }: This defines a function named create_user that creates a new user using the useradd and passwd commands.

list_users() { ... }: This defines a function named list_users that lists all regular users using the getent passwd command.

list_sudo_users() { ... }: This defines a function named list_sudo_users that lists users with sudo permissions using the getent passwd command and filtering the output.

function get_file_info() { ... }: This defines a function named get_file_info that gets information about a file such as size, permissions, owner, and last modified time using the stat command.

The script then parses the command-line arguments using conditional statements.

If the --version option is provided, it displays the version number using echo.

If the --help option is provided, it calls the display_help function to display the usage information.
If the cpu getinfo option is provided, it calls the get_cpu_info function.

If the memory getinfo option is provided, it calls the get_memory_info function.

If the file getinfo option is provided, it calls the get_file_info function with the filename and additional options.

If the user create option is provided, it calls the create_user function with the username.

If the user list option is provided, it calls the list_users function. If the --sudo-only option is provided, it calls the list_sudo_users function instead.

If none of the recognized options are provided, it displays an error message using echo and exits the script with an exit code of 1.

    

<img width="431" alt="Screenshot 2023-11-02 at 7 29 21 PM" src="https://github.com/Kd4u/INTER-LINUX-COMMANDS/assets/96914340/f6a70ed4-43c1-4596-adb6-93614de53c8b">
