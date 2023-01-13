# zigup
manage zig compiler versions

Inspiration comes from rustup and pyenv. 

I discovered https://github.com/marler8997/zigup after I had written a POC in Python.

## Usage

fetch a compiler and set it as the default

```shell
zigup <version>
  
zigup master
  
zigup 0.6.0
```

fetch a compiler only (do not set it as default)

  
```shell
zigup fetch <version>
  
zigup fetch master
```

print the default compiler version

  
```shell
zigup default
```
  
Set the default compiler

  
```shell
zigup default <version>
```
  
list the installed compiler versions


```shell
zigup list
```
  
clean compilers that are not the default, not master, and not marked to keep. when a version is specified, it will clean that version

  
```shell
zigup clean [<version>]
```

mark a compiler to keep

  
  
```shell
zigup keep <version>
```
  

run a specific version of the compiler

  
```shell
zigup run <version> <args>...
```

display the path to the given command

```shell
zigup which <command>
```

