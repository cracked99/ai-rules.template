# Cursor Rules Cookiecutter Template

A cookiecutter template for creating projects with pre-configured Cursor rules for AI assistance.

## Features

- Pre-configured `.cursor` folder with AI assistance rules
- Standard project structure
- Development environment configuration
- VSCode settings
- GitHub Actions workflow
- Devcontainer configuration

## Usage

### Prerequisites

- Python 3.6 or higher
- [Cookiecutter](https://cookiecutter.readthedocs.io/en/latest/installation.html) (`pip install cookiecutter`)

### Creating a New Project

To create a new project using this template, run:

```bash
cookiecutter gh:yourusername/cursor-rules-template --checkout template
```

Replace `yourusername` with your actual GitHub username.

### Template Variables

When you run the cookiecutter command, you'll be prompted to provide values for the following variables:

- `project_name`: The name of your project
- `project_slug`: The directory name for your project (auto-generated from project_name)
- `project_description`: A short description of your project
- `author_name`: Your name
- `author_email`: Your email address
- `version`: Initial version of your project
- `open_source_license`: License for your project

## License

This template is available under the MIT License. 