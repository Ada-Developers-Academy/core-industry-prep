# A Github PR Review

In this section we will walk through the code review process using Github pull requests.  Git is the most common version control system and Github the largest hosting service for git repositories.  Thus Github makes a good starting point for practicing code reviews.  

Much of the steps and etiquite of a code review apply across systems however.

## The Mechanics of a Github PR Review

### Requesting a PR

As you begin working on a feature [start the feature on as branch](https://www.git-tower.com/learn/git/faq/create-branch).  It's also a good idea to check and make sure you are using linters and tools to help enforce your team's adopted style guide.  This will prevent stylelistic errors and help reviewers focus on what the code is doing.  You should also try to keep the changes as small and focused as possible.  It is much easier for reviewers to understand and evaluate changes when they are of modest size.

Before you make a pull request make sure that:

1. The code compiles/executes successfully
1. The code is adequately tested
1. You have examined the changes yourself one final time.

When your feature is ready push all changes up to github:

```bash
$ git push origin <BRANCH_NAME>
```

Then go to github and find your branch and click on the `New Pull Request` button.

![New Pull Request Button](images/new-pull-request.png)

Then add a description to your PR describing the feature and rationale for the changes.  Communicate the changes clearly.  Add any open questions you still have about the feature.  Then you can use gear icon under reviewers to request a code review.

![Request Code Review](images/request-reviewers.png)

## Reviewing Code in Github

To review a pull request on the github webpage first click on the `files changed` tab.  

![files changed tab](images/files-changed.png)

Then you can examine the proposed changes.  You can click on a `+` sign next to any line of code to add inline comments.  The comments are in [markdown](https://guides.github.com/features/mastering-markdown/) format.  

Good code review comments can be:

- Questions to the author about the purpose or need for the code.
- Suggestions for improvements
- Compliments

It is important to remember that the code belongs to the team, use the word "We" over "You" and feel free to criticise the code, while being respectful of the author.  **Be specific** in your comments or questions.  You can add code samples to illustrate your point.  Remember that your comments in a code review are **suggestions** and not commands.  

When you have finished reviewing the PR, click on the `Review Changes` button and leave a summary of your impressions and either approve or request changes for the review

![Review Changes Button and summary textbox](images/review-changes.png)