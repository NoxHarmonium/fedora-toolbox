# fedora-toolbox
Additions to the default fedora-toolbox image that I commonly use

## Summary

I use Fedora Silverblue for my developer machine and I love using toolboxes.
However, it's a pain to have to install common developer tools everytime I create a toolbox.

These images bake in the tools I commonly use to make my life easier.

## Building

```shell
# or whatever version you're on
cd f40
podman build -t fedora-toolbox:40 .
```

## Using

```shell
toolbox create -i localhost/fedora-toolbox:40 foo
```