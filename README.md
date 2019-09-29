# Description

This is an incomplete sample VUE.js application which displays British Columbia Aquifer data by location.

## Code Challenge instructions

This code challenge will confirm your ability to assess and implement requested changes to an application and submit code changes through Pull Requests.

You will find 2 issues reported in this repository; complete both by submitting separate pull requests for each issue.

Do not publish this code to a public repository.

### Data

Aquifer data is in a static JSON file in [/src/data](src/data).

### Code Challenge Evaluation Rubric

The application code will be assessed using the following criteria:  

| Points  | Criteria |
|---|---|
| 10 pts | Bug issue fixed |
| 30 pts | Enhancement issue added and working as expected |
| 15 pts | Definition of Done met |
| 10 pts | Acceptance criteria met |
| 10 pts | Unit/lint tests pass |
| 10 pts | Git used effectively (commits, PRs, branches) |
| 15 pts | Code is simple, elegant, commented and easy to understand |
| 100 pts | TOTAL |

## Project setup

Ensure NPM and NODE are installed.

```sh
npm install
```

### Compiles and hot-reloads for development

```sh
npm run serve
```

### Compiles and minifies for production

```sh
npm run build
```

### Run your tests

```sh
npm run test
npm run test:unit
```

### Lints and fixes files

```sh
npm run lint
```

### Customize configuration

See [Configuration Reference](https://cli.vuejs.org/config/).

## Instructions for Code Challenge Administrator

1. Clone the code to a private repository on GitHub
2. Go to the repository Settings > Options and ensure option 'Template repository' is checked
3. Go to the 'Code' tab and 'Use this template' to make copies of the repository
4. Re-create the following 2 issues to all copies of the repo

### Issue #1: View aquifer details by location (Enhancement)

#### Story

As a Well Driller, I need to view a list of aquifers in a location so that I will know where to safely drill a new well.

#### Acceptance Criteria

Given I select a location from the drop-down  
When a location is selected  
Then one or more aquifer details are displayed on the screen in a table

#### More information

Replace the 'Selected location' alert box with a table displaying the following fields:  

```sql
aquifer_id | mapping_year | name | area | vulnerability
```

In most cases, only one aquifer will return. Location: 'Cassidy' should return more than one for example.

#### Definition of Done

- Bootstrap Vue styles used
- Lint no errors
- Unit test coverage

### Issue #2: List does not order by lower and upper case (Bug)

#### Description

The SELECT box doesn't order items A-Z properly. Lowercase items display at the end of the list.

#### Steps to Reproduce

- Run the application
- On the home page, click on the Aquifers select box
- Scroll to bottom of list
- Expected Result
- Items are sorted alphabetically.

#### Actual Result

Lowercase items at bottom.

#### More Information

The original developer noted that a related 'Check alpha order' unit test is failing when running 'npm run test:unit'. This test should pass when the issue is fixed.
