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

The tip of the `master` branch of the project is what goes to production. To contribute, use [fork + pull request](https://help.github.com/articles/fork-a-repo/) workflow. Avoid creating your own branches in the project repository.

##### Code Reviewing

All code needs to be reviewed before it is merged back to the `master` branch.

1. Pull the branch in question.
2. Run it locally.
3. Inspect the code changes and offer any tips on how it may well be improved
4. If you're happy with it then add a "+1" comment.

With two "+1" comments on any given Pull Request the original creator is free to approve the Pull Request.

Consider switching your `master` branch to be a [protected branch](https://help.github.com/articles/about-protected-branches/), which will make reviews mandatory.

### Task breakdown & Issue Tracking

We create github issues. Anyone is free to add issues to any given Project.

Once a developer begins working on an issue they assign themselves to it so others know it is in progress.

Use [milestones](https://help.github.com/articles/creating-and-editing-milestones-for-issues-and-pull-requests/) to create and track burndown (aka deadline-based) lists of issues.

#### Testing and Continuous integration

Consider developing a testing plan for your project. What are the things that matter and need to be checked twice before pushing to prod? For example, the project [i-like-hillary-but](https://github.com/DevProgress/i-like-hillary-but) is mostly articles with links, so an [html-proofer](https://github.com/gjtorikian/html-proofer) is a good way to make sure the links lead the user to the right places.

A healthy project could use a hygiene robot that watches over it. We use [Travis CI](https://travis-ci.org/profile/DevProgress) and it's really easy to set up. There are straightforward [guides](https://docs.travis-ci.com/) available.

You need to be an admin of the project in order to flip the *Travis CI* switch. Ask for the privilege or ping one of the folks on `#peeps-infra`.

### Deploying

We use [Github Pages](https://pages.github.com/) for deployment. To set up:

1. Set up your development workflow to write production files to the `/docs` directory. Though the name seems like a bit of a misnomer, using it provides the least cumbersome Github Pages deployment option. Here are some examples:

  1. Jekyll on [`i-like-hillary-but`](https://github.com/DevProgress/i-like-hillary-but/blob/master/_config.yml).
  2. React+WebPack on [`debate-bingo`](https://github.com/DevProgress/debate-bingo/blob/master/webpack.config.js).

2. Follow [instructions](https://help.github.com/articles/configuring-a-publishing-source-for-github-pages/#publishing-your-github-pages-site-from-a-docs-folder-on-your-master-branch) for publishing Github Pages site from a `/docs` folder on your `master` branch.

3. Whenever you're ready to deploy, write the latest production files into `/docs`, commit them to `master`, and follow the usual code review process. It may take a bit of time for Github Pages to update.
