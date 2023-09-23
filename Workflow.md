# Portfolio 2: Workflow

This is the second entry to the portfolio, where I will be focusing on the tasks given by my lecturer, Brian Davison.
The tasks for this week are to show that I know how to use the workflow tools in [GitHub](https://github.com/), 
as well carrying out a series of operations on GitHub.

I will do this by making use of screenshots and providing detailed explanations where necessary. 

Afterwards, I will reflect on these tasks and discuss any difficulties faced while doing them and how I resolved them.

## Workflow Tools

The tools which were made use of are contained within this [GitHub Flow](https://docs.github.com/en/get-started/quickstart/github-flow) 
and the information inside is what my team has agreed upon. It should also be known, that the team is making use of a [Kanban Board](https://www.atlassian.com/agile/kanban/boards)
using a webite called [Zube.io](https://zube.io/docs) which has been integrated with the teams GitHub repository. We are also making use of [Discord](https://www.discord.com) for active communication.

The kanban board, described simply, is an online taskboard, where tasks can be listed and people with access to the board can take a task and do it.
They come with a lot of additional functionality and flexability, for example, we chose the sections we wanted to list and gave them names. It is able
to update GitHub in real time, which makes tracking issues and who is resolving them easy to see. 

## Tasks

The tasks I received are as follows:

- Accept a task from the project backlog
- Update the task information appropriately
- Update the task board appropriately
- Complete the development task on a feature branch
- Commit your changes with appropriate comments
- Check your work against the Definition of Done (DoD)
- Make a pull request

I will tackle each of these tasks in order and where necessary, provide screenshots.

### Accepting a task

Accepting a task from the project backlog on GitHub is easy due to the kanban integration. Simply click the
"Issues" button at the top of the GitHub repository to view the active issues. Then, you can choose the issue 
to work on, then when the task is chosen, you can assign yourself to the task, as shown below.

| ![3 steps to assign](images/Assigning.png "This shows the 3 steps involved to assign a task to yourself") |
|:--:|
| <b> Fig.1 - 3 steps to assign a task in GitHub </b> |

### Update the task information

Before or after accepting the task, the user is able to leave a comment. It may be reasonable to leave a comment
with the date that you take the task, as well as when you would expect to hand it in.

### Update the task board appropriately

Updating the task board is made easy with kanban, it can be done on both GitHub and Zube.io. Since the previous example
was shown on GitHub, I will show the process on Zube.io for this step. Below is an image of the kanban board our team is using
on Zube.io.

| ![kanban board](images/Zube.png "The kanban board.") |
|:--:|
| <b> Fig.2 - The kanban board on Zube.io </b> |

As is clearly visible, the kanban board has numerous boxes, and users with access are able to drag and drop
each post into any box they need to, which allows the user to easily update the status of their task. I moved
the task I wanted to tackle into the "In progress" section. 

### Complete the development task on a feature branch

To achieve this, first the user would open the branches section of the GitHub repository, then, they would create their own branch to work on.
The team have agreed on a desired naming system for doing this. It is as follows - feature_name/firstname-surname-ID-issue_number. As can be seen below,
this is how my one looks.

| ![Issue name as branch](images/IssueImg.png "My issue branch name.") |
|:--:|
| <b> Fig.2 - This image shows the task I chose as the branch. </b> |

Afterwards, I opened my Visual Studio and changed the branch on the shared team repository to the name of the branch I created as shown below.

| ![Shared repo branch change](images/ChangeRepo.png "Changing branch.") |
|:--:|
| <b> Fig.2 - This image shows where to change branch name, and that I have done it. </b> |

To do this, click the dropdown and select "Remote" and the branch should be listed. However, if it is not, you may need to sync
again before trying.

Also, the task I chose was to create a program which would allow the user to add, view, update and delete different types of equipment from
a local database. I achieved this by using the .Net Maui framework in Visual Studio, and SQLite to create the local database. I will not cover
this further, as it is not required. 

### Commit the changes with appropriate comments

To commit the changes, we do it on the same page displayed above, where we changed the branch.
Committing the changes means that the changes will be made locally and not made on the GitHub repository yet.
I will add comments to show that the project has been completed and added to a separate folder, to allow anyone
who looks at it to know what I have added and how to access it as seen below.

| ![Committing the changes.](images/Commit.png "Comments and commit.") |
|:--:|
| <b> Fig.2 - This image shows where the user would commit, as well as appropriate comments </b> |



