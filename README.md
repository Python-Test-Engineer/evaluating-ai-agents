# The Pytest Cookbook - *recipes with videos and repos*

## Purpose of this book 

To provide a range of ready congfigured PYTHON TEST FRAMEWORKS with a 'one step install', comprising of templates and references for developers to adapt to their own needs.

To provide curated resources of articles, videos and books that I have found useful.

Frameworks, apps and folders may well have additional README.md files to give more detailed instructions.

## Test Suites

These can be set up as follow:

`python -m venv venv`
`pip install -r requirements.txt`
`playwright install` for API and BDD suites as we need to load in browsers for Playwright
`python -m pytest -vs` - there is pytest-sugar for prettier output

*See the README.md in root of each Test Suite for detailed and up to date set up instructions.*

These four are incremental, with each suite adding more functionality to the previous one:

- PyTest_00_MINIMAL - a basic src folder wired to PyTest with custom logging and pytest-sugar console formating.
- PyTest_01_PYTEST - as above but with a large number of ready made test templates demoing how to use PyTest along with templates for Mocking and Patching.
- PyTest_02_API - as above with API testing and Playwright e2e/functional testing.
- PyTest_03_BDD - as above with Behavior Driven testing that enables the use of native English test requirement files to be wired to PyTest and Behave Framework. BDD enables all stakeholders to work on these 'feature' test files in plain English which are then translated to Python test code.

These are self-contained Test Suites:

- PyTest_04_DB_TESTING - is a standalone test suite for testing database schemas such as foreigh keys, constraints, nullability etc. Uses SQLModel (SQLAlchemy + Pydantic) to inspect DB. Uses SQLite as test DB and this has some restricted schema information but there are tests for thes.
- PyTest_05_DJANGO is its own unique testing suite built from a range of sources. 
- PyTest_06_HYPOTHESIS is a standalone property based test suite that can provide templates and resources on how to use property based testing. It can be thought of as very extensive parameter based testing to test edge cases and hone in on them.
- PyTest_07_PLUGIN - this is a template PyTest plugin project for adaptation.
- PyTest_08_HOOKS - a small project outputing information on hooks and what they provide.
- PyTest_09_CLI - testing a Typer CLI project.
- PyTest_10_CI_CD - a CI/CD example to show how we can use GitHub actions to test our code base on multiple Python versions and OS. May be replaced with TOX.
