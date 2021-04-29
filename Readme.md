Including a remote resource base before a base using CRD merging breaks the merging.

```shell
> kustomize build ok | grep 'my-special-image'
    - image: my-special-image
> kustomize build broke | grep 'my-special-image'
# no match
```
