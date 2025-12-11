# Github Collaboration Exercise

How to collab in Github, using merge strats and CI/CD workflows

## Purpose

This repo is for myself (and hopefully for others) to experiment and learn how collaboration is to be carried out using Github. This exploration includes:

1. How to adopt merge strategies when making changes. Some strats are explained below.
2. Using CI/CD + testing workflows with Github Actions. This is something known, but new for me.

### Why?

Because I've been confused and have yet to receive any formal mentoring/guide on how to do these stuffs. I do however, remember how things were done in my past **team project** back in university and that was hands down the best experience working properly in a team setting. 

Even though I was actively participating, I missed out some parts especially when formulating CI/CD workflows for our repo back then, so here I am trying to do it by myself. Also we used GitLab back then and not Github but honestly, just different tools different terminologies and workflows.

### What I've already known so far

I know about *some* branching/merging strategies as wll as basic understading of what CI/CD is.

1. I know what a merge request (pull request) is.
2. I know how to merge branches and solve conflicts.
3. I know how to open an issue, but in Github, a branch will not be made automatically upon opening it unlike GitLab (where you can can also customise the name format of your branch).
4. I know how make feature branches and the feature branching strategy.
5. I understand how approving pull requests work.
6. I understand how CI/CD pipeline works in general. I don't know how to set it up just yet.

As such, I want to try emulate the kind of workflow I did back when I had my amazing team project. I loved the proper, clean and collaborative workflow we had back then and want to come up with a personal 'cookbook' or 'wiki' on how to start it or just understand it whenever I join another project/team.

As I progress through doing stuffs in this repo, I will update this README on the go.

## Proposed tech stack

I'm planning to use **Vite** with vanilla JS as my basic tech stack. A frontend web dev should be enough.

Why Vite? I simply want to test the CI/CD and testing workflows on something with node.js. Could've used something else like Java or C\# which I'm more familiar with but I want to keep it as simple as possible... hopefully..

## Test #1 - Opening an issue

Opened an issue [here](https://github.com/nykten/github-collab-exercise/issues/1) with tagging and assigning myself as the assignee. Simple enough. Maybe lack direction but that's how it's simply done.

You apparently can't tie an issue with a branch (or create one) within the issue page unlike GitLab.

Based on observation on other repos including OSS repos, most people describe their 'issues' with any improvements/bugs/feature request that could be added to the repo, then just create a branch themselves. Then, they would push their commits to the remote repo while opening a pull request. This way, they can also 'link' or more precisely *'add reference'* of the issue to the pull request.

Example seen in: [This pull request](https://github.com/firebase/functions-samples/pull/1214).
They mentioned the issue in the pull request as *"Fixes #[issue-number]"*

### Workflow differences (GitLab vs Github)

#### GitLab:

1. Open an issue.
2. Can select the option to automatically create a new branch with the issue name.
3. Make changes and commit to the branch created.
4. Push to remote repo.
5. Make a merge request (PR).
6. Solve merge conflicts if any,
7. Merge request clears CI/CD pipeline & approvals.
8. Merge to main/master.

#### Github:

1. Open an issue describing the issue/new feature.
2. Make a new branch manually (locally/remotely).
3. Make changes, commit & push to the branch.
4. Make a pull request.
5. Solve merge conflicts if any.
6. Pull request clears CI/CD pipeline & approvals.
7. Merge to main/master.

### Takeaway

So the only difference in the workflows would be the automation of creating a branch upon an issue creation in GitLab while Github doesn't have that. Although I think it might be possible with some integrations.

Not much of an issue or confusion, just that I like the workflow on GitLab better.

