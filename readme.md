# How to develop IVY / IVY Template / Bedrock

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