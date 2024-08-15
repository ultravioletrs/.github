# Contributing to Ultravioletrs

The following is a set of guidelines to contribute to Ultraviolet and its repositories, which are hosted on the [Ultravioletrs Organization](https://github.com/ultravioletrs) on GitHub.

This project adheres to the [Contributor Covenant 1.2](http://contributor-covenant.org/version/1/2/0).
By participating, you are expected to uphold this code. Please report unacceptable behavior to
[info@ultraviolet.rs](mailto:info@ultraviolet.rs).

## Reporting issues

Reporting issues is a great way to contribute to the project. We are perpetually grateful for a well-written, thorough bug report.

Before raising a new issue, check the issues page to determine if it already contains the problem that you are facing.

A good bug report shouldn't leave others needing to chase you for more information. Please be as detailed as possible. The following questions might serve as a template for writing a detailed
report:

- What were you trying to achieve?
- What are the expected results?
- What are the received results?
- What are the steps to reproduce the issue?
- In what environment did you encounter the issue?

## Pull requests

Good pull requests (e.g. patches, improvements, new features) are a fantastic help. They should remain focused on scope and avoid unrelated commits.

**Please ask first** before embarking on any significant pull request (e.g. implementing new features, refactoring code etc.), otherwise, you risk spending a lot of time working on something that the maintainers might not want to merge into the project.

Please adhere to the coding conventions used throughout the project. For Golang-based repos, if in doubt, consult the [Effective Go](https://golang.org/doc/effective_go.html) style guide.

To contribute to the project, [fork](https://help.github.com/articles/fork-a-repo/) it, clone your fork repository, and configure the remotes:

```bash
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>
git remote add upstream https://github.com/ultravioletrs/<repo-name>.git
```

If your cloned repository is behind the upstream commits, then get the latest changes from upstream:

```bash
git checkout main
git pull --rebase upstream main
```

Create a new topic branch from `main` using the naming convention `COCOS-[issue-number]` for cocos related issues to help us keep track of your contribution scope. For other repositories, use the naming convention `UV-[issue-number]`:

```bash
git checkout -b UV-[issue-number]
```

Commit your changes in logical chunks. When you are ready to commit, make sure to write a Good Commit Message™. Consult the [Erlang's contributing guide](https://github.com/erlang/otp/wiki/Writing-good-commit-messages) if you're unsure of what constitutes a Good Commit Message™. Use [interactive rebase](https://help.github.com/articles/about-git-rebase) to group your commits into logical units of work before making it public.

Note that every commit you make must be signed. By signing off your work, you indicate that you
are accepting the [Developer Certificate of Origin](https://developercertificate.org/).

Use your real name (sorry, no pseudonyms or anonymous contributions). If you set your `user.name`
and `user.email` git configs, you can sign your commit automatically with `git commit -s`.

Locally merge (or rebase) the upstream development branch into your topic branch:

```bash
git pull --rebase upstream main
```

Push your topic branch up to your fork:

```bash
git push origin UV-[issue-number]
```

[Open a Pull Request](https://help.github.com/articles/using-pull-requests/) with a clear title
and detailed description.
