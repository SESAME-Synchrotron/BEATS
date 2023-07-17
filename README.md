# BEATS
This repo is sub-module based repo that includes all BEATS related repos in one place. 

- To add a new sub-repo to BEATS repo: 
``` 
git submodule add <BEATS_related_repo_url>
```
- Cloning a Repository with Submodules:
If you want to clone this repo with all sub-modules: 
```
git clone git@github.com:SESAME-Synchrotron/BEATS.git
cd BEATS
git submodule update --init --recursive
```
- Updating Submodules:
When you pull changes to your main repository that include updates to the submodules, you need to update the submodules as well. Use the following command:
```
git submodule update --remote
```
This command fetches and applies changes from the remote repository of each submodule.
