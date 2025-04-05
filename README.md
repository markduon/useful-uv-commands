# useful-uv-commands
This repository includes some common and useful commands of UV - an extremely fast Python package and project manager, written in Rust.

```bash
1. Create a new Python project:
uv init <PROJECT-NAME>

2. Alternatively, you can initialize a project in the working directory:
mkdir <PROJECT-NAME>
cd <PROJECT-NAME>
uv init

3. Run a command or script:
uv run main.py

4. Add dependencies to the project:
# Add multiple specific dependencies
uv add numpy pandas

# Add all dependencies in requirements.txt file
uv add -r requirements.txt

5. Remove dependencies:
uv remove pandas

6. Save all dependencies in current working project into requirements.txt:
uv export --no-hashes --format requirements-txt > requirements.txt

7. Update the project lockfile:
uv lock

8. Update the project environment:
uv sync

9. Display the project dependency tree:
uv tree

10. Manage Python versions and installations:
# List the available Python installations
uv python list

# Download and install Python versions
uv python install 3.13

# Use a specific Python version in the current directory
uv python pin 3.13
```