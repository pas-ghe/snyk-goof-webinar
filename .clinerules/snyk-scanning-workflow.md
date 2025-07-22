## Brief overview
These guidelines outline the workflow for using Snyk to scan for security vulnerabilities during development. This ensures that new code and dependencies are scanned, and any identified issues are remediated before completion.

## Snyk Scanning Workflow
- When new first-party code is written, run Snyk Code to identify any security vulnerabilities in the code.
- When new dependencies are added or existing ones are updated, run Snyk Open Source (SCA) to check for vulnerabilities in the open-source packages.
- Only fix security issues that are introduced by the new or modified code and dependencies. Do not address pre-existing vulnerabilities that were not part of the recent changes.
- After applying a fix, rescan the code or dependencies to verify that the vulnerability has been successfully remediated.
- Ensure that the fix does not introduce any new security issues.
- Continue this process of scanning and fixing until no new issues are detected in the modified code or dependencies.
- At the end of the task, provide a summary of the number of security issues that were found and how many were successfully fixed.
