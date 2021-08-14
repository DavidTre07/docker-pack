# Features

## Implemented

- [x] Recursively find dependencies of binaries passed in argument
- [x] Ability to define the docker TAG and/or VERSION
- [x] Ability to define uid:gid or user of whih the docker will run
- [x] Ability to provide a template Dockefile
- [x] Ability to give a file as parameter where all binaries are listed
- [x] Ability to don't build automaticaly the docker (leave the files ready to build)
- [x] Ability to define the working directory
- [x] Define ENTRYPOINT and/or CMD
- [x] Ability to add fonts inside docker so some apps that need fonts sill works
- [x] Build process logging in a file
- [x] Ability of making DNS resolution (nslookup)
- [x] Ability to define a user in the docker (passwd file)
- [x] Add an init bin (tini used) so all signals are well handled
- [x] Check if docker image with same name and tag exist, if yes refuse to build the image

## To do

- [ ] If UID or user specified then, when copying files inside docker, add chown option in the COPY instruction
- [ ] In the case of a script, read the script to find all binaries/libs used inside and pack it all
  - [x] Shell (bash, sh, ksh, ...)
  - [ ] Python
- [ ] If a script call another script, analyse the dependencies recursively

Open to new ideas !!!!
