# Submodules

Update 1: 
`.gitmodules` is not tracking a specific branch of `Portfolio`
So this repository's submodule will always point to master, unless someone changes 
the branch it points to in `.gitmodules`

Update 2: Changed the branch tracking in `.gitmodules` from `master` to `submodule_test`

Update 3: Manually adding branch tracking doesn't work, have to use `git submodule add -b <BRANCH_NAME> <REPO_URL>`
Deinitializing submodule...

Update 4: Reinitializing Submodule with Branch Tracking

Update 5: Switched branch inside submodule to `master`
	Github continues to track `submodule_test` branch

Update 6: Switched branch inside `.gitmodules` to 'master'

Final Update: Using submodules without branch tracking is more flexible, when a user is working on a different branch, when pushed, the submodule will be pushed to the new branch. When a new user clones the repository, the submodule will be empty. They will be required to run `git submodule init` followed by `git submodule update` to update to the specific branch of the submodule.
