Docker may be used to build RPatchur through containers.
Through Docker, the build process contains all necessary dependencies.

To build RPatchur with Docker, complete the following procedure:
```shell
# Build the RPatchur build container
$ cd /path/to/rpatchur/docker
$ docker image build -t rpatchur .

# Use the rpatchur image to build rpatchur
$ docker run -v /path/to/rpatchur:/rpatchur rpatchur
$ file /path/to/rpatchur/target/x86_64-pc-windows-gnu/release/rpatchur.exe
/path/to/rpatchur/target/x86_64-pc-windows-gnu/release/rpatchur.exe: PE32+ executable (GUI) x86-64, for MS Windows
```
