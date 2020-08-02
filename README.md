# git-workflow
I have deisgn below git architecture for Zendriix Softwares to address the issue for timely release.
I have provided the branching details,creation and it usage.

1. Master branch: this branch will be created by default after the git repo initilization. This branch will accomodate the final copy of the code after every release. Current release branch will be merged to master after every release.

2. Develop branch: this branch will be created from master initially and respective features and relase branch will be created from Develop branch. once  feature branch has all the code ready for the release, code will be merged to develop and from develop code will be merged to release branch. Develop will be our default branch. 

3. Feature branch: For every release , new feature branch (feature/<release date> ) will be created from develop and merged to develop, If we have to exclude any thing from release that is in develop already than we can separate the branch from feature and merge to release directly. This will be an exception.
  
4. Release Branch: this branch will be created from develop for every release, if any thing has to be excluded from develop in some exceptions, we will merge the code direclty to release from feature.

