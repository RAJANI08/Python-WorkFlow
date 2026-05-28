# Python-WorkFlow
1.Push code to GitHub → workflow starts automatically.
2. Checks out your code.
3. Installs Python 3.12.
4. Restores/downloads cached pip packages (faster builds).
5. Installs dependencies from requirements.txt.
6. Runs main.py.
7. Saves the output to output.txt.
8. Uploads output.txt as an artifact that you can download from the workflow run.

# Cache vs Artifact in this Flow

# Cache 

Saves installed packages.
Next workflow run is faster.
Example: Flask already downloaded, no need to download again.

# Artifact 

Saves generated files.
Example: test reports, logs, build files.
Can be downloaded after the workflow finishes.

Easy interview answer:

Cache: Stores dependencies to speed up future workflow runs.
Artifact: Stores files produced by a workflow for later download or use.
