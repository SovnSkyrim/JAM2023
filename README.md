# R-Type Project

This project contains a server (binary: r-type_server) and a client (binary: r-type_client) for the R-Type game.

## Compilation

The project uses CMake for compilation. Follow the steps below to compile the project:
 - 1: Run the following git commands to initialize submodules:

```
git submodule init
git submodule update
```

 - 2: Create a build directory:

```
mkdir build
cd build
```
 - 3: Ensure that you have CMake installed. If not, you can install it using:

```
sudo apt-get install cmake
// OR
sudo dnf install cmake
// OR
pacman -Syu cmake
```

 - 4: Generate configuration files with CMake:
```
cmake ..
```
 - 5: Compile both server and client using the command:
```
make
```


## Usage

Once the compilation is complete, you can run the server and client using the following commands:

   You can run the server using the command:

    make serv

   You can also specify a port for the server by adding the PORT argument during compilation:

    make serv PORT=8080

   You can run the client using the command:

    make cli

   For the client, you can specify the port and server IP address:

    make cli PORT=8080 SERVER_IP=127.0.0.1

   If the client is on a different machine, the IP will be the IP address of the PC in its network

    make cli PORT=8080 SERVER_IP=85.168.161.236


## Engine documentation

[Click on this link](EngineReadme.md)