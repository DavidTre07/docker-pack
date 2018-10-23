* If instead of uid:gid the user provide username then grab uid and gid in passwd file
* Fonts: instead of hard coded font path, detect which fonts are installed and pack it if requested
* When passwd file generated the user shell is nologin, so we need to add it to the binaries to pack in the docker
* In the case of a binary that is symlinked to another binary (for example sh is a symlink to bash), then pack the right binary and create symlink