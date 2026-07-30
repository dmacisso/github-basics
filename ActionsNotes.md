## Section 3. GitHub Actions - Basic Building Blocks & Components

![alt text](/github-basics/images/image.png)

### Lesson 37. Creating a First Workflow

[Github Repository: github basics](https://github.com/dmacisso/github-basics/tree/main)

Actions => Simple Workflow => configure button
Path: github-basics/.github/workflows/first-action.yml in main

```yml
name: First Workflow
on: workflow_dispatch # waits for user to manually start
jobs:
  first-job:
    runs-on: ubuntu-22.04
  steps:
    -  name: print greeting
      run: echo "Hello World!"
    -  name: print goodbye
      run: echo "Done Goodbye"
```

- select commit button
- to github-basics/.github/workflows/first-action.yml 
- we executed a commit to the repository 

![alt text](/github-basics/images/image1.png)

[Github action events](https://docs.github.com/en/actions/reference/workflows-and-actions/events-that-trigger-workflows)

### 42. Actions

- Action is a separate feature of Github actions.
  - A (custom) application that performs (typically complex) frequently repeated tasks
  - Fetching the code from github and downloading it on a "runner" machine.
  - Can be distributed through a marketplace


- Command (using run keyword)
  - Alternative to an action.
  - simple shell commands written in a yml file
  - also can run scripts on runner machine

- [Search for github actions checkout](https://github.com/actions/checkout).

  -  click marketplace 
  -  verified actions by Github team

### 43. Checking Out Code in Workflows

[github runners](https://docs.github.com/en/actions/concepts/runners)
