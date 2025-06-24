GitLens Detective – HTTPie CLI

This repository contains my submission for the GitLens Detective challenge.
The goal was to use the GitLens extension in VS Code to analyze the commit history of a specific function in an open-source project.

--------------------------------------------------
Challenge Objective

Using the GitLens extension in VS Code, the challenge required identifying:

- Who wrote a particular function
- When it was last updated
- What commit or PR added it

--------------------------------------------------
Project Analyzed

Repository: https://github.com/httpie/cli
File: httpie/internal/daemon/daemons.py
Function Investigated: _start_process()

--------------------------------------------------
Findings

Function: _start_process()

Author:          Batuhan Taskaya
Created On:      May 5, 2022
Commit Message:  Automatic release update warnings
Pull Request:    https://github.com/httpie/cli/pull/1336

Additional Modification:

Modified By:     Sadik Kuzu
Modified On:     May 19, 2022
Commit Message:  Fix typos in comment lines
Pull Request:    https://github.com/httpie/cli/pull/1405

--------------------------------------------------
Repository Structure
````text

.
├── gitlens_insights.md               # Detailed GitLens analysis
├── README.md                         # Challenge overview (this file)
└── screenshots/
    ├── _start_process.png  # Author: Batuhan Taskaya
    └── blame_view_comment_fix.png    # Modified by: Sadik Kuzu
````
--------------------------------------------------
How to Reproduce

1. Clone the repo:
   git clone https://github.com/httpie/cli.git
   cd cli

2. Open the project in Visual Studio Code.

3. Install the GitLens extension (if not already installed).

4. Navigate to:
   httpie/internal/daemon/daemons.py

5. Hover over the _start_process() function to see author and commit info using GitLens.

--------------------------------------------------
