## riff init node

Initialize a node.js function

### Synopsis

Generate the function based on the function source code specified as the filename, using the name
and version specified for the function image repository and tag.  

For example, from a directory  named 'square' containing a function 'square.js', you can simply type :

    riff init node -f square

  or

    riff init node

to generate the required Dockerfile and resource definitions using sensible defaults.

```
riff init node [flags]
```

### Options

```
  -h, --help   help for node
```

### Options inherited from parent commands

```
  -a, --artifact string          path to the function artifact, source code or jar file
      --config string            config file (default is $HOME/.riff.yaml)
      --dry-run                  print generated function artifacts content to stdout only
  -f, --filepath string          path or directory used for the function resources (defaults to the current directory)
      --force                    overwrite existing functions artifacts
  -i, --input string             the name of the input topic (defaults to function name)
      --invoker-version string   the version of the function invoker to use when building containers (default "latest")
  -n, --name string              the name of the function (defaults to the name of the current directory)
  -o, --output string            the name of the output topic (optional)
  -u, --useraccount string       the Docker user account to be used for the image repository (default "current OS user")
  -v, --version string           the version of the function image (default "0.0.1")
```

### SEE ALSO

* [riff init](riff_init.md)	 - Initialize a function

