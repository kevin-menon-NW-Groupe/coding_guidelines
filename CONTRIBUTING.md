# Submit changes
docs: https://nw-tech.atlassian.net/l/cp/4AUxfvHM
bugs: issue tracker / bug report tool
comms: [C05HBCTSW00](https://app.slack.com/client/T036G49CL9Y/C05HBCTSW00)

# Environment

## Docker
No need for Poetry, since all in docker is isolated, even the python runtime
Make the docker containers more lightweight by not installing development dependencies
Third-party packages should be reduced to a minimum ideally, to avoid long pip installations, slow docker startups and storage overhead.

# Template usage
You can kickstart a project using the following templates:
 - https://github.com/NW-Tech/nwre-fastapi-python-docker-template

However, once generated, be sure to personallize it and delete portions unnecessary. This will make it easier for maintainers to know which parts to focus on.


## Config file
.env with examples in .env.example

## Database

### Database ORM
We use SQLALchemy

### Database migrations
alembic

alembic migrations --autogenerate
alembic upgrade head

# Testing

## Unit tests


# Coding conventions
Based on https://google.github.io/styleguide/pyguide.html


## Coding style
Black, used by pre-commit

### Type hints
Mypy will ensure everything is statically typed

## Symbols (variables, classes, functions, etc.)


# Documentation
All functions should have a docstring formatted in MD.
technical documentation can be uploaded on Confluence with a plugin.

# Review

# Versionning

## Git commits
Conventional commits, all in English

## Git branches
Follow Git flow conventions

## PR and reviews
name of the PR should mention the JIRA ticket as a prefix. Ideally, the merge of the ticket into dev should squash the source commits into one

## JIRA issues

# Integration
Tests should be on Github Actions.
We need a few automatons and a real "integration" environment.

# Deployment

