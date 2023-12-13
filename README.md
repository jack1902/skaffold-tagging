# skaffold-tagging

Run the below for similar output:

```sh
➜ skaffold build --dry-run
Generating tags...
 - test -> test:02624bc
```

Then with the `v1.0.0` commit, you should get the following build-tag from skaffold `v1.0.0`

```sh
➜ skaffold build --dry-run
Generating tags...
 - test -> test:v1.0.0
```

For commits past the `v1.0.0` tag, you will see things similar to this:

```sh
➜ skaffold build --dry-run
Generating tags...
 - test -> test:v1.0.0-1-HASH
```
