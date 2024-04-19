# ROADMAP

### [Swiffty CLI](https://example.com)
The swiffty CLI helps to create plugins with ease. Use a few simple commands to begin developing.
- [X] Basic CLI structure using clap 
- [X] Command manager
- [X] Print Swiffty on command
      
 ### Init Command
- [X] Create manifest.toml
- [X] Create src/index.lua
- [X] Create .gitignore
- [X] Init git repo

### Build Command
- [ ] Check manifest.toml options for correct plugin options
- [ ] Check git repo for uncommited changes
- [ ] Read .gitignore to find ignored directories
- [ ] Create /build
- [ ] Check for existing release in /build
- [ ] If existing plugin version in /build, delete it
- [ ] Zip files and add it to /build in format {name}@{version}

