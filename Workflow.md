    // drafting...
  
# Intro

DevProgress is a team of kick ass developers using their skills and expertise to create tools that will help elect Hillary Clinton and other Democratic and progressive candidates.

Here is outline of our standard break down of tasks, pushing code and releasing to production.

## Tooling

### Tech stack.

Our standard baseline code is lightweight client only react web apps on gh-pages.

- Javascript. 
- React. Javascript driven css.
- Webpack npm dev and build.
- Automated Testing (?)
- Continuous Delivery (?)

### Trello

Trello is used to track all our projects at a high level.

It's not something we use to track tasks at a project level.

_This is where ideas and campaign requests are first created._

Developers can visit the trello board to see what projects are new, inflight and done.

### Slack

Slack is our discussion forum for all projects. 

_This is where technical decisions get made._

Developers can use slack to join the conversation around any particular project and discover how they can help.

### Github

Once a technical approach has been agreed upon in slack the collaboration moves to github to track tasks, branch and code review.

#### Branching Strategy

We only really have 2 types of branches.

1. Master. This is what goes to Production.
2. _Whatever branch you are working on_. This is where you start by branching of master.

#### Pull Request: Code Review & Merge

To get your work back to the Master branch you will need to create a Pull Request and have 2 people add a "+1" comment on it.

##### Code Reviewing

All code needs to be reviewed before it is merged back to the `master` branch.

1. Pull the branch in question.
2. Run it locally.
3. Inspect the code changes and offer any tips on how it may well be improved
4. If you're happy with it then add a "+1" comment.

With two "+1" comments on any given Pull Request the original creator is free to approve the Pull Request.

### Task breakdown & Issue Tracking

We create github issues. Anyone is free to add issues to any given Project.

Once a developer begins working on an issue they assign themselves to it so others know it is in progress.

### Testing

...

### Deploying

Github Pages.

Our strategy for merging from `master` to `gh-pages` is currently a work in progress. Tbc.