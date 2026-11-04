# Software Requirements Specification - Starter Structure

Use the content of this repository as a starter template for developing your Software Requirements Specification SRS.

The SRS document can be found under [Main](Main.md) 

## How to adopt
* As a group git-admin, fork this GitHub repository to your own account.
	* Make your repository private and do not share with other groups.
	* Add your fellow group members as collaborators.
* Clone the repository to your own local computer.
* In Obsidian, go to `Manage Vaults... -> Open Folder as Vault` and then select the folder where your local clone is located.

## How to update

* Edit in Obsidian as per directions and advice with regards to structures, traceability links, meta-data.
* Follow commit practices recommended below throughout.
* `git push` your commits as needed for other members to see.
* **Other members: `git pull` before editing anything.** Let everyone know what you are editing to avoid conflicts.
* Commit often and once done, do a last pull then push.

### Commit Practices
* Adopt the commit template that can be found in `.gitmessage`
* Adopt as follows
	* `git config commit.template .gitmessage.txt`
* **First step: pull from GitHub!**
	* `git pull`
* Edit as appropriate
* Add files to the index using 
	* `git add [files]`
* Commit by simply doing
	* `git commit`
	* The editor will open with the template loaded according to `.getmessage.txt`
	* Customize the message, save and close for the commit to complete.
* **You may need to do multiple commits in one seating if you have done many distinct changes to facilitate subsequent tracing.**

## Query your repo
### Query (whatever is in) Working Directory

- Use grep. In MS Windows, it is accessible through opening Git Bash.
- Examples:
	- Which requirements are in progress?
		- `grep -rli "^status:.*in progress" --include="*.md" .`
	- Requirements for which john must be informed:
		- `grep -rlPzi '(?s)author:(?:(?!\n\w).)*\bjohn\b' --include="*.md" .`
	- Use cases that yet don’t have tests:
		- `grep -rLE "^related-tests:\s*\S" --include="*.md" ./uc`

### Query repository
- Use `git log [params]`
- Examples:
	- Get me the history of a file:
		- `git log --follow -- path/to/file.md`
	- Get me a diff of what has changed in the file:
		- `git log -p -- path/to/file.md`
	- Commits relating to a specific Jira task:
		- `git log --follow --grep="LMS-123" -- path/to/file.md`
	- Follow the rationale of the changes:
		- `git log --grep="rationale:" --format='%h | %(trailers:key=rationale,valueonly)’ -- path/to/file.md`

