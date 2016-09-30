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

We use [Github Pages](https://pages.github.com/) for deployment. To set up:

1. Set up your development workflow to write production files to the `/docs` directory. Though the name seems like a bit of a misnomer, using it provides the least cumbersome Github Pages deployment option. Here are some examples:

  1. Jekyll on [`i-like-hillary-but`](https://github.com/DevProgress/i-like-hillary-but/blob/master/_config.yml).
  2. React+WebPack on [`debate-bingo`](https://github.com/DevProgress/debate-bingo/blob/master/webpack.config.js).

2. Follow [instructions](https://help.github.com/articles/configuring-a-publishing-source-for-github-pages/#publishing-your-github-pages-site-from-a-docs-folder-on-your-master-branch) for publishing Github Pages site from a `/docs` folder on your `master` branch.

3. Whenever you're ready to deploy, write the latest production files into `/docs`, then commit and push them to `master`. It may take a bit of time for Github Pages to update.
