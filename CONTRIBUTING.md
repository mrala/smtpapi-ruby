Hello! Thank you for choosing to help contribute to one of the SendGrid open source libraries. There are many ways you can contribute and help is always welcome. We simply ask that you follow the following contribution policies.

- [Improvements to the Codebase](#improvements-to-the-codebase)
- [Understanding the Code Base](#understanding-the-codebase)
- [Testing](#testing)
- [Style Guidelines & Naming Conventions](#style-guidelines-and-naming-conventions)
- [Creating a Pull Request](#creating-a-pull-request)
- [Code Reviews](#code-reviews)

<a name="improvements-to-the-codebase"></a>
## Improvements to the Codebase

We welcome direct contributions to the smtpapi-ruby code base. Thank you!

### Development Environment ###

#### Install and Run Locally ####

##### Prerequisites #####

- Ruby version 2.2
- The SendGrid Service, starting at the [free level](https://sendgrid.com/free?source=smtpapi-ruby))

##### Initial setup: #####

```bash
git clone https://github.com/sendgrid/smtpapi-ruby.git
cd smtpapi-ruby
```

##### Execute: #####

See the [examples folder](examples) to get started quickly.

To run the example:

```bash
ruby examples/example.rb
```

<a name="understanding-the-codebase"></a>
## Understanding the Code Base

**/examples**

Working examples that demonstrate usage.

**/tess**

Unit tests

**/lib/smtpapi**

Source code.

<a name="testing"></a>
## Testing

All PRs require passing tests before the PR will be reviewed.

All test files are in the [`test`](test) directory.

For the purposes of contributing to this repo, please update the [`test.rb`](test/test.rb) file with unit tests as you modify the code.

To run the tests:

```bash
rake test
```

<a name="style-guidelines-and-naming-conventions"></a>
## Style Guidelines & Naming Conventions

Generally, we follow the style guidelines as suggested by the official language. However, we ask that you conform to the styles that already exist in the library. If you wish to deviate, please explain your reasoning.

- [Community Driven Style Guide](https://github.com/bbatsov/ruby-style-guide)

Please run your code through:

- [rubocop](https://github.com/bbatsov/rubocop).

## Creating a Pull Request<a name="creating-a-pull-request"></a>

1. [Fork](https://help.github.com/fork-a-repo/) the project, clone your fork,
   and configure the remotes:

   ```bash
   # Clone your fork of the repo into the current directory
   git clone https://github.com/sendgrid/smtpapi-ruby
   # Navigate to the newly cloned directory
   cd smtpapi-ruby
   # Assign the original repo to a remote called "upstream"
   git remote add upstream https://github.com/sendgrid/smtpapi-ruby
   ```

2. If you cloned a while ago, get the latest changes from upstream:

   ```bash
   git checkout <dev-branch>
   git pull upstream <dev-branch>
   ```

3. Create a new topic branch (off the main project development branch) to
   contain your feature, change, or fix:

   ```bash
   git checkout -b <topic-branch-name>
   ```

4. Commit your changes in logical chunks. Please adhere to these [git commit
   message guidelines](http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html)
   or your code is unlikely to be merged into the main project. Use Git's
   [interactive rebase](https://help.github.com/articles/interactive-rebase)
   feature to tidy up your commits before making them public.

4a. Create tests.

4b. Create or update the example code that demonstrates the functionality of this change to the code.

5. Locally merge (or rebase) the upstream development branch into your topic branch:

   ```bash
   git pull [--rebase] upstream main
   ```

6. Push your topic branch up to your fork:

   ```bash
   git push origin <topic-branch-name>
   ```

7. [Open a Pull Request](https://help.github.com/articles/using-pull-requests/)
    with a clear title and description against the `main` branch. All tests must be passing before we will review the PR.

<a name="code-reviews"></a>
## Code Reviews

If you can, please look at open PRs and review them. Give feedback and help us merge these PRs much faster! If you don't know how, Github has some great <a href="https://help.github.com/articles/about-pull-request-reviews/">information on how to review a Pull Request.</a>
