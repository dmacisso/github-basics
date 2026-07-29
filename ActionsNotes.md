## Section 3. GitHub Actions - Basic Building Blocks & Components

![alt text](/images/image.png)

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