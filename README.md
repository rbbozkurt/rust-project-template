<img src="https://github.com/rbbozkurt/rust-project-template/assets/45459787/fe3f0cbf-1def-4747-bed2-6895dfa0b8d6" width="1000" height="800">

# Rust Project Template


Welcome to our Rust Project Template! This template is designed to make starting a new Rust project as easy as possible. It includes everything you need to get going quickly, including setup scripts, essential tools, and basic configuration files like README.md.template and LICENSE.template. The goal is to help you focus on writing your Rust code without worrying about the initial setup.

## Table of Contents

- [Installation](#installation)
  - [Prerequisites](#prerequisites)
  - [Setup](#setup)
- [Usage](#usage)
  - [Local Setup](#local-setup)
  - [Using Codespaces](#using-codespaces)
- [Features](#features)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Installation

### Prerequisites

Before beginning, ensure you have installed:

- Git
- GitHub Copilot (optional, but recommended for enhanced coding assistance)

### Setup

To use this template, follow these steps:

1. Navigate to the [rust-project-template](https://github.com/rbbozkurt/rust-project-template) on GitHub.
2. Click the "Use this template" button located at the top-right of the page.
   ![image](https://github.com/rbbozkurt/rust-project-template/assets/45459787/688f02f1-6c7d-456f-b4b1-865213a4bbc5)


3. Follow the prompts to create a new repository based on this template.

## Usage

### Local Setup

To set up the project locally:

1. Open a terminal and navigate to the directory where you wish to clone the repository.
2. Clone your new repository using `git clone https://github.com/<your-username>/<your-repo-name>`.
3. Change into your repository's directory with `cd <your-repo-name>`.
4. (Optional) Create and switch to a new branch with `git checkout -b <branch-name>`.
5. Run `./setup.sh` to install necessary dependencies and perform initial setup.

### Using Codespaces

For Codespaces:

- The `setup.sh` script will automatically execute upon starting your Codespace, as configured in `.devcontainer/devcontainer.json`.

### Rust Version Configuration

The script `setup.sh` configures the environment to use Rust version `1.74.0` by default. If you need to use a different Rust version for your project, you can easily specify this by running the setup script with the desired version number as an argument. For example, to set up Rust version `1.55.0`, you would use the following command:

```bash
./setup.sh --rust 1.55.0
```
### Python Version Configuration

Similarly, the script is set up to configure the environment to use Python version `3.10` by default. If your project requires a different Python version, you can specify this by providing it as the second argument to the setup script. For instance, to set up Python version `3.9`, along with the default Rust version, you would run:

```bash
./setup.sh --python 3.9
```
### Specifying Both Versions

If you need to specify both Rust and Python versions, you can provide both `--rust` and `--python` flags with their respective version numbers. For example, to set up Rust version `1.55.0` and Python version `3.9`, the command would be:

```bash
./setup.sh --rust 1.55.0 --python 3.9
```
These named argument configurations provide a clear and flexible way to set up your environment according to the specific requirements of your project.

## Features

This Rust project template comes with several pre-configured features designed to to kickstart development, enhance code quality, and ensure a consistent coding environment.

- **Dev Container for Codespaces**: Provides a fully configured development environment with all necessary dependencies and tools. This feature enables developers to start coding immediately without worrying about local setup, making it ideal for collaborative projects and quick starts.

- **Automated Rust Environment Setup**: The template automatically installs Rust, its compiler (`rustc`), the package manager (`cargo`), and other essential tools such as `rustfmt` for code formatting and `clippy` for linting. This ensures that every developer works with the same toolchain, reducing "works on my machine" issues.

- **Pre-configured Clippy and Rustfmt**: Integrates Rust's official linting tool (`clippy`) and formatting tool (`rustfmt`) to enforce code quality and style consistency. This helps maintain high code standards and reduces time spent on code reviews related to style issues.

- **Pre-commit Hooks**: Utilizes `pre-commit` hooks to automatically check and format code before commits, ensuring that all code complies with defined standards and preventing common errors from being committed to the repository.

- **Continuous Integration (CI) Setup**: Includes a basic setup for Continuous Integration (CI) using GitHub Actions, automating tasks like building the project, running tests, and linting code on every push or pull request. This helps in identifying and resolving issues early in the development cycle.

- **README and LICENSE Templates**: Includes `README.md.template` and `LICENSE.template` files to guide the creation of comprehensive project documentation and ensure proper licensing right from the start. The README template outlines how to structure project information, making it easier for new users to understand and contribute to the project. The LICENSE template provides a placeholder for legal protection and clarifies the terms under which the software can be used, modified, and distributed.

- **Automated Documentation Deployment**: The `deploy_docs.yml` workflow in GitHub Actions automates the deployment of your project's documentation to GitHub Pages. Whenever changes are pushed to the main branch, the documentation is automatically built and deployed, ensuring that your project's documentation is always up-to-date with the latest codebase. This seamless integration enhances the project's maintainability and accessibility for both developers and users.

- **Extensible Template**: While this template provides a solid foundation for Rust projects, it's designed to be easily extensible. Developers can add more tools, libraries, and configurations as needed, making it suitable for projects of any scale.

By leveraging these features, developers can focus more on building their applications and less on configuring and maintaining their development environment.


## Contributing

Contributions are welcome! Here's how you can contribute:

- **Bug Reports**: If you notice a bug, please open an issue with a clear title and description.
- **Feature Requests**: Have an idea for improvement? Feel free to open an issue to suggest new features.
- **Pull Requests**: Direct contributions can be made by forking the repository, making your changes, and submitting a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

For questions or feedback, please contact [resitberkaybozkurt@gmail.com](mailto:resitberkaybozkurt@gmail.com).
