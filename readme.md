# How to develop IVY / IVY Template / ZOM / Bedrock

* clone the repo
* pull in the submodules
    
    git submodule update --init --recursive
      
* For each project being edited, checkout a new branch there and run the builds, e.g.

    cd _ttio_templates/ivy
    git checkout -b my-branch
    npm run dev #TODO what is the actual command for each one?
    
    
Submodules include
_plugins-core
_ttio_templates/zom
_ttio_templates/bedrock
_ttio_templates/ivy

When changes are made to a submodule, commit those changes in that submodules folder and push those changes to the respective repo on your branch (adding a tag and merging to master if ready for a release).

In the main repo (IVY), you'll also want to create a commit that points IVY to the new commit you just made for the submodule. Push to your branch on github or qa, master, production if the IVY starter repo in those environments should be updated to point to the new submodule commit/version you made.
