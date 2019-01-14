# vivo-template

This template creates a 3 tier build for a local CU Boulder VIVO installation.
It checks out Vitro, VIVO, and then vivo-cuboulder in the target directory.
It also checks out facetedsearch, which is used for the people and publication pages for VIVO.

When this repo is checked out, each of the submodules will be initialized at a certain commit hash. You see this when you cd to one of the submodules and then with the "git branch" command see "no branch".
The setup.sh script overcomes this by checking out all submodules to the current branch.
This script can be run directly, or can be used as a guideline by executing each of the lines individually.

Handling updates to submodules.
When there are updates to a submodule like vivo-cuboulder. The submodule needs to be added to the template and then committed.
Still uncertain if this should be done for every branch, or if we can just apply it to master following successful acceptance of the required changes in the submodule.
