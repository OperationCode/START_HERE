# Introduction to GitHub for Educational Institutions

Item                    | Requirement
---                     | ---
Class time              | 90 minutes
Intended Audience       | High school and higher-ed classrooms
Pre-requisite knowledge | Web browsing literacy
Materials               | Access to GitHub.com, and an e-mail address for verification
Delivery medium         | This class can be taught face-to-face or remotely (synchronous)

## Learning Outcomes

By the end of this lesson, students will be able to:

- Create an account on GitHub.com
- Describe features of a distributed version control system
- Use Issues to track their own progress
- Use GitHub Flow to add a hometown file
  - Create branches
  - Add commits on the web UI
  - Open a pull request
  - Collaborate through light code reviews
  - Ship the addition of your hometown file
- Explore projects hosted on GitHub

## Set Up
- Create a class repo with the following in the README.md file:
  - Instructor names and contact information
  - Markdown guides (see Resources/Mastering Markdown)
- Add students as collaborators using one of the following two methods:
  1. Manually add each student as a collaborator using the repo Settings > Collaborators.
  2. Create an issue for students to comment on at beginning of class and while class is in session, you or a teaching partner can run the [add-collaborators](https://github.com/github/training-utils/blob/master/add-collaborators) script that's part of our [training-utils](https://github.com/github/training-utils).

## Materials
- Guide introducing [GitHub Flow](https://guides.github.com/introduction/flow/)
- Learn git by Michael Hartl's [Learn Enough Git to be Dangerous](https://www.learnenough.com/git-tutorial)
- Illustrations on [Version Control Systems](https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control) and on [Committing and History](https://git-scm.com/book/en/v2/Getting-Started-Git-Basics) from *Pro Git*
- [Training Kit](https://services.github.com/kit/) and its [repo](https://github.com/github/training-kit)
- [Training Utilities](https://github.com/github/training-utils)
- [Mastering Markdown](https://guides.github.com/features/mastering-markdown/)

## Outline

Time        | Topic
---         | ---
5 minutes   | Introduce motivation for why version control is necessary. Some examples: sending draft copies of papers back and forth to friends and teachers, collaborating with others on a blog, sharing and building upon recipes.
5 minutes   | Contrast centralized and distributed version control systems (VCS), highlighting the benefits of a distributed VCS (DVCS). Assert that Git is a DVCS.
5 minutes   | Contrast Git and GitHub. Call out the features of GitHub that are not present in Git.
10 minutes  | Demonstrate logging into GitHub, the dashboard, and the Code, Issues, and Pull Requests tabs of the repo you created for class work.
5 minutes   | Describe the permissions of a collaborator and how it differs from a visitor to the project. Show the Settings tab of a repo and how to add collaborators manually. Then, depending on how you chose to add students as collaborators, either (1) let students know they've been added as collaborators or (2) ask students to comment on your collaborator issue while you or a teaching partner runs the script that will add commenters as collaborators.
5 minutes   | Describe the steps of GitHub flow. Explain that collaboration is the core component of the workflow.
10 minutes  | Demonstrate how to create an issue. Students should follow along. Use the demonstration as an opportunity to describe Markdown and showcase the use of the toolbar for beginners, describe how labels might be used to tag and sort conversations. In the title of the issue, have each student include their username, which will make it easier to cross-link when a Pull Request (PR) is opened later. In the body of the issue, have each student summarize the steps of GitHub Flow using a task list. Create the issue, and show how assignees can be used to denote ownership of an issue.
5 minutes   | Draw contrast between Issues and Pull Requests. Describe that an issue was used to track our progress and possibly start a conversation that may or may not lead to change in the code. Mention that Pull Request, on the other hand, must contain work along with the conversation, which enables code review.
5 minutes   | Demonstrate and have students follow along as you create a branch. Highlight the differences between the new branch and `master`. Ensure students include their username in the branch name so there are no conflicts with branch naming. The branch name should also contain the student's hometown.
5 minutes   | Demonstrate and have students follow along as you create a town for your hometown. Ensure students uniquely name the file with their username and their hometown, using the format [username]-[hometown], so that no merge conflicts occur. The file should use the Markdown extension. Add content to the file with some information about the your and the students' hometown.
5 minutes   | Commit your changes and describe a commit as a snapshot of the code at the time the commit was created. Ensure students are committing only to their branch.
5 minutes   | Review the pull request and describe the 3 tabs that make up a PR.
10 minutes  | Ask students to find the PR directly below theirs on the list of open PRs, and navigate through their classmates' tabs to review the proposed hometown file. Show students how to collaborate and leave comments, highlighting at-mentions and line comments. Ask students to include `:+1:`, `:ship:`, or `:shipit:` to indicate to their classmates their file is ready to ship.
5 minutes   | Demonstrate how to merge the changes proposed in the PR. Explain how the history on the feature branch now lives on `master` and showcase how student files appear on master.
5 minutes   | :tada: Celebrate! Congratulate students for their first contribution and describe iterative development. Highlight projects on GitHub open to contributions, and the Project Showcase.
