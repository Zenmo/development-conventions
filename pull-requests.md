# Format

The pull request format is the same as the [Commit format](https://nextcloud.zenmo.com/apps/collectives/Development-2/Commit-format-5492).

# Scope

A pull request should contain a coherent changeset.

Different kinds of changes should be in separate PR's. For example:

- New feature
- Refactoring
- Code style change
- Bugfix

# Size

Pull requests have a soft size limit of 1000 lines.

# Process

- The change author creates the pull request
- The author assigns one or more reviewers
- The reviewer does the review 
  - There can be one or more rounds of feedback and changes
- At least one approve is required
- The change author merges the commit 
  - This is done through a rebase to get a linear history
  - Squashing is optional but recommended.
  - All commits which end up in the main branch must conform to the [Commit format](https://nextcloud.zenmo.com/apps/collectives/Development-2/Commit-format-5492).

# Responsibility

It is the responsibility of the author to follow the process, find willing reviewers, and get approves.

An approve does not imply that responsibility for the impact of the change is shared with or offloaded to the reviewer.

# Commits

A pull request can be one or more commits.