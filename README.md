# Wget Wizard (Offline)
This is [Wget Wizard](https://www.whatismybrowser.com/developers/tools/wget-wizard/) but offline. This singular HTML file is literally everything. That's it.

It has every option from the original: URL, entire directory, complete mirror, crawl depth, URLs-in-file, file type filters, metadata-file skipping, if-exists behavior, output directory, resume, robots/cert/cache toggles, retries, wait and random wait, fake user agents, referrer, logging, verbosity and short/long syntax. The command updates live as you change options, so there’s no submit step.

A couple of new features:
- A shell selector for bash/zsh, PowerShell or Windows cmd. This changes how the command is quoted.
- A multi-line toggle that wraps the command with the right line-continuation character for the chosen shell.
- Copy and Save as script buttons.
- Warnings for risky combinations, such as a directory URL without a trailing slash, or resume together with timestamping.

Choosing “entire directory” works out the ```--cut-dirs``` number from the URL for you. Directory and mirror are mutually exclusive, and mirror uses your crawl depth instead of unlimited depth.
The user agent strings are hardcoded, so they will go stale over time. You can update them in the ```USER_AGENTS``` object near the top of the script.

Screenshot

<img width="726" height="980" alt="wget1" src="https://github.com/user-attachments/assets/290dc42b-0797-4b46-b4f5-1ce30c79fab7" />
