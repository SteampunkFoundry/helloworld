# helloworld

The most basic of Java programs. A simple Java application that compiles to a
`.jar` file using Maven.

## Building

```bash
mvn clean package
```

## Running

```bash
java -cp target/helloworld-1.0.jar com.steampunk.helloworld.HelloWorld
```

## Pre-commit hooks

[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)

This repository enables Git pre-commit hooks using the [pre-commit framework](https://pre-commit.com/).
These hooks are client-side and must be enabled by each developer.

To enable them for your use, you must have Python installed and then you can
install pre-commit with `pip install pre-commit`. (Some Linux systems might
need to use `pip3 install pre-commit`.) Once Python and pre-commit are
installed, you can enable a repository that has a `.pre-commit-config.yaml`
file by typing `pre-commit install` within the repository.

After that, the pre-commit hooks listed in `.pre-commit-config.yaml` must pass
on any changed files before the commit can be successfully completed. You can
[temporarily disable](https://pre-commit.com/#temporarily-disabling-hooks) a
hook by adding a `SKIP` environment variable.

Be aware that some hooks will reformat files when the pre-commit hook fails,
meaning that attempting the commit immediately will be successful. However, you
are encouraged to review the changes the hooks make to ensure they are
appropriate and don't break anything.
