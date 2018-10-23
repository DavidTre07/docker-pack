# docker-pack: Put a software inside a docker easily

This script will put inside a docker the binary(ies) of your choice.  
It will generate the docker image without the need to create a Dockerfile.  
It manage to put inside the docker all libs needed by the artefact.  

<b>Usage:</b>
```
./docker-pack [-a file] [-b] [-c cmd] [-d] [-e cmd] [-f file] [-h] [-l log_file] [-n] [-p user] [-s template_file] [-t tag] [-u uid:gid] [-v version] [-w workdir] binary [binary] [binary] [binary]

-a file : A listing of files to add inside the docker image (absolute path, one file per line)
-b      : Don't build the docker
-c cmd  : Define command to run on docker CMD
-d      : Debug mode
-e cmd  : Define entrypoint (default: 1st binary)
-f      : Add font inside docker
-h      : This Help
-l file : Log into a file
-n      : Activate nslookup
-p user : Activate password file with an account provided as parameter
-s file : Dockerfile template file (if not provided a default one will be generated)
-t tag  : Define Docker image tag (default: 1st binary name)
-u uid:gid : Define a uid:gid as docker will run (USER in dockerfile)
-v version : Define Docker image version (default: 1.0)
-w workdir : Working directory (default: /tmp/docker-pack)
Binary(ies) to put inside a docker

Example: ./docker-pack /usr/bin/tar
         To run it: docker run --rm tar:1.0 --help

```
