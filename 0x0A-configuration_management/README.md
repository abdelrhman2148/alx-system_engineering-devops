# Configuration Management with Puppet

This project focuses on utilizing Puppet as a powerful configuration management tool. Puppet enables the automation of tasks related to system configuration, ensuring consistency and reliability across multiple nodes in a network.

## Tasks Overview 📃

### 0. Create a File

**0-create_a_file.pp**: This Puppet manifest file is designed to create a file named "school" in the `/tmp` directory with specific permissions, group, owner, and content.

- **File Permissions**: 0744
- **File Group**: www-data
- **File Owner**: www-data
- **File Content**: "I love Puppet"

### 1. Install a Package

**1-install_a_package.pp**: This Puppet manifest file facilitates the installation of the Flask package from pip3, a Python package manager.

### 2. Execute a Command

**2-execute_a_command.pp**: This Puppet manifest file orchestrates the execution of a command to kill a specific process.

---

By employing Puppet for configuration management, these tasks can be efficiently automated, ensuring system integrity and facilitating scalable infrastructure management.
