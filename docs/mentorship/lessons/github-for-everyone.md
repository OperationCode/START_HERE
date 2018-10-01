# GitHub for Everyone
Lesson Plan

Item                    | Requirement
---                     | ---
Class time              | 2.5 - 3 hours
Intended Audience       | High school and higher-ed classrooms
Pre-requisite knowledge | Web browsing literacy
Resources               | Access to GitHub.com, an e-mail address for verification, GitHub Desktop application, and network permission to interact with Git and GitHub
Delivery medium         | This class can be taught face-to-face or remotely

## Learning Outcomes

By the end of this lesson, students will be able to:

- Create an account on GitHub.com
- Describe features of a distributed version control system
- Use Issues to track their own progress
- Use GitHub Flow to add a hometown file
  - Create branches on the web UI and on GitHub Desktop
  - Add commits on the web UI and on GitHub Desktop
  - Open a pull request
  - Collaborate through light code reviews
  - Sync changes between local environment and remote
  - Resolve Merge Conflicts in GitHub Desktop
  - Ship the addition of your hometown file
- Explore projects hosted on GitHub

## Set Up
- Create a class repo with the following in the README.md file:
  - Instructor names and contact information
  - Markdown guides (see Resources/Mastering Markdown)
- Add students as collaborators using one of the following two methods:
  1. Manually add each student as a collaborator using the repo Settings > Collaborators.
  2. Create an issue for students to comment on at beginning of class and while class is in session, you or a teaching partner can run the [add-collaborators](https://github.com/github/training-utils/blob/master/add-collaborators) script that's part of our [training-utils](https://github.com/github/training-utils).
- All student computers should have GitHub desktop installed.  

## Resources
- Guide introducing [GitHub Flow](https://guides.github.com/introduction/flow/)
- Learn git by Michael Hartl's [Learn Enough Git to be Dangerous](https://www.learnenough.com/git-tutorial)
- Illustrations on [Version Control Systems](https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control) and on [Committing and History](https://git-scm.com/book/en/v2/Getting-Started-Git-Basics) from *Pro Git*
- Creating a perfect pull request [How to write the perfect pull request](https://github.com/blog/1943-how-to-write-the-perfect-pull-request)
- Creating a perfect git commit message [How to write a Git Commit Message](http://chris.beams.io/posts/git-commit/)
- Merge Conflicts [Resolve simple merge conflicts](https://github.com/blog/2293-resolve-simple-merge-conflicts-on-github)
- [Training Kit](https://services.github.com/kit/) and its [repo](https://github.com/github/training-kit)
- [Training Utilities](https://github.com/github/training-utils)
- [Mastering Markdown](https://guides.github.com/features/mastering-markdown/)

## Outline

### Getting Started with Collaboration - ~25 minutes

| Time |Activity |
|-----------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 5 minutes | Ask class to make sure they have Desktop installed from desktop.github.com. Ask and answer the question "What is GitHub?" Explain key GitHub features, and the differences between GIt and GitHub. Explore a repository and cover each view of code, issues, and pull requests. Discuss special file types, like `README.md`.
| 10 minutes | Show where to add collaborators in the Settings page, let learners know we'll add them with a script using the GitHub API. Create a new issue and demonstrate markdown for headers, checkboxes and emoji. @mention any co-teachers. Show the preview, and that Issues can include attachments. Ask learners to comment on issue. To add students as collaborators, either add them manually or with a script found in the open source `training-utils` repository called `add-collaborators`. If using the script, have students comment on an individual issue. You can also assign the issue to a co-teacher and add a label to showcase these features and their use. |
| 2 minutes | Learners will start getting a lot of email notifications. Take this opportunity to show the 3 ways to manage notifications - by issue/pull request, by repository, or general. |
| 5 minutes | Cover GitHub Flow using the GitHub Flow Guide. Tell students we'll practice following GitHub Flow while adding information about our hometowns. Then, demonstrate and have them follow along as you open an issue listing the steps of GitHub Flow. Each student will do the same to track their own progress. This is a good time to outline the learning objectives as well as review markdown syntax. |

### Practicing GitHub Workflow - ~40 minutes

| Time |Activity |
|-----------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 2 minutes | Show how to create a branch (the first step in GH Flow), and have students follow along as you create a branch 'username-hometown' |
| 2 minutes | Demonstrate and have each student follow along in their own branch as you create a Markdown file on GitHub with information about your hometown. Commit the file to your branch. Return to your tracking issue to check off the corresponding steps in the progress |
| 10 minutes | Describe a pull request, and create a Pull Request on GitHub. Show `base:` and `compare:` drop downs, highlight the `Conversation`, `Commits`, and `Files changed` view. Create a line comment and add a general comment to the discussion. Have the students do the same on a partner's open Pull Request. |
| 5 minutes | Edit the file based on the pull request comments. Commit the file changes. Show the `Commits` tab with the new commit.  |
| 2 minutes | Merge your open Pull Request. Describe what happens when we merge Pull Requests. Have students follow along to merge their own pull requests. Check off the remaining items in the tracking issue and close it. Delete the branch |
| 5 minutes | Switch to using GH Desktop, spend some time ensuring the students are logged in to Desktop. Clone the repository and explain the purpose of a clone. |
| 2 minutes | On Desktop, create branch on  called username-desktop |
| 2 minutes | Make changes and commit them on the new branch. Show file on master without changes and check out the new branch to highlight the file with changes. Explain the two-stage commit. |
| 2 minutes | Explain publish/sync, publish the changes, create a PR from published changes |


### Merge Conflicts - ~50 minutes

| Time |Activity |
|-----------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 5 minutes | Create a new branch, called conflict-branch.         |
| 5 minutes | Make changes to your original file                   |
| 5 minutes | Return to master, make changes to master.            |
| 6 minutes | Start a PR between master and conflict-branch.       |
| 3 minutes | Note issue, create PR anyways.                       |
| 2 minutes | Return to Desktop. Switch to conflict branch.        |
| 4 minutes | Update from Master button (creates a merge locally). |
| 6 minutes | Open with editor. Resolve conflict.                  |
| 4 minutes | Return to desktop. Submit commit and publish/sync.   |
| 2 minutes | Return to .com, complete PR                          |
| 5 minutes | Discuss merge conflict principles                    |
