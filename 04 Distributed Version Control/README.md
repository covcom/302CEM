
# Distributed Version Control

Each week you will be expected to complete a series of lab activities. You will be required to reflect on these in your assignment so make sure you keep records of what you have done. The supporting presentation can be found at https://goo.gl/HtacrJ

## Configuring GitLab
By now you should have started to implement your first user story so you will already have some code under development. In this first task you will be putting this code under version control to help track changes and manage issues.

1. Make sure all of your team members have a GitLab account and have added their full name and photo to their user profile.
2. One of your team should log into GitLab, select Groups from the left-hand navigation and create a new group using your team name.
  1. Under the group Settings, add your group details and upload a suitable avatar.
3. On the Group page use the Members section, invite the other team members to join, assign them Developer permissions.
4. Create a repository to hold your application code and make sure all your team members can see it on GitLab.com

## Cloning the Repository
Now it's time for each developer to get a copy of the repository in order to start development.

1. You should use the Terminal if you are working on a Mac or Linux device (including cloud-based IDEs) or The Git Bash application if you are using Windows.
2. One team member should navigate to the directory where they want to store their local repository and clone the remote repository using the git clone command.
  1. This will create a directory containing the empty repository.
3. Drag the latest project files into this directory.
4. Add, commit and push the files to GitLab. Check gitlab.com to make sure these have been successfully pushed.
5. The other team members can now clone the repository, they all now have a complete copy of the repository and its files.

## Setting Milestones
Milestones allow your team to assign deadlines and assign issues to them.

1. From the project screen select the Milestones option.
2. Create four milestones dated two weeks apart and named Sprint 1, Sprint 2, Sprint 3, Sprint 4.

## Feature Branching
Each feature (based on a user story) should be developer on a separate branch. In this section of the worksheet you will learn how to manage this process.

1. Start by opening the remote repository on gitlab.com and locating the Issues tracker.
  1. Add an issue for each user story in the Sprint Backlog, this will assign it a unique tracking number.
  2. Assign each issue to the Sprint 1 milestone.
  3. Write this number on the user story cards (and on the Trello cards)
2. One member of the development team should now create a local branch and switch to it.
  1. Write some code then add and commit this to the new branch.
  2. Push all branches back to the remote.
  3. Check that there are  now two branches in the GitLab remote.
3. The other members of the team can now pull all remote branches into their local repository and switch to the feature branch.
4. All team members can now contribute to the development of this feature branch.

## Merge Request
Once a feature has been implemented on a feature branch it needs to be merged back into the master branch. The activities here should be undertaken once your team are confident that the feature has been fully implemented and tested.

1. One member of the team responsible for the feature implementation should trigger the Merge Request.
  1. On the GitLab project screen choose the Merge Request option.
  2. Under Source Branch select the feature branch you want to merge.
  3. Under Target Branch choose the Master branch.
  4. Click on Compare branches and Continue.
2. You will need to provide a title and a description.
3. You will also need to assign it to the project owner (the person who created the repository) and the correct milestone.
4. The person designated as reviewer should be able to see the merge request.
  1. They can review the proposed changes.
  2. If they are happy that the feature has been implemented they can approve the merge request.
  3. This will merge the changes into the master branch and delete the issue branch.
  4. The feature branch will still be in the local repository so this will need to be deleted.

## Project Forking
This is an advanced distributed workflow which is suited to large numbers of collaborators. It allows multiple development teams to collaborate on a single project in a carefully controlled manner. You will need to work closely with the other teams in order to implement it.

1. Choose which team will lead on the development. They need to provide the other team's GitLab admin user with Guest permissions.
2. The second team admin person should be able to access the project home page.
3. They click the Fork button and fork the project into their team's group.
4. Now the other members of this second group can clone this repository and contribute code to this.
5. The original read-only repository will need to be added as a second upstream remote and any changes pulled, then pushed to the team remote to keep it in sync.

### Merge Request
After implementing a user story, the second team can make a merge request.

1. They need to specify a branch in their forked repository as the Source Branch.
2. They need to specify the Master branch in the original read-only repository as the Target Branch.

## Using Other Remote Repositories
All the activities in this worksheet are based around GitLab however they apply equally to other platforms that implement the Git Version Control system. You are encouraged to try out these techniques with:

1. GitHub
2. BitBucket

# Git Flow

Need to install

Then initialise inside an existing repository.
```
git flow init
```

## Features

Start a new feature.
```
git flow feature start myfeature
```

Share a feature with other developers
```
git flow feature publish myfeature
```

Get a feature from the remote to work on.
```
git flow feature pull origin myfeature
```

Track feature on remote.
```
git flow feature track myfeature
```

Finish a feature.
```
git flow feature finish myfeature
```

## Releases

To start a release use the following. It creates a release branch from the develop branch.
```
git flow release start myrelease
```
Then need to publish the release branch to allow other developers to contribute.
```
git flow release publish myrelease
```
Track the remote release.
```
git flow release track myrelease
```
Finishing up a release. remember to push the tags.
```
git flow release finish myrelease
git push --tags
```

https://yakiloo.com/getting-started-git-flow/

http://danielkummer.github.io/git-flow-cheatsheet/
