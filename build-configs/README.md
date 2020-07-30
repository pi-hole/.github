# Build configuration files for CI/CD

## Travis-CI

Travis-CI can source [shared build configurations](https://docs.travis-ci.com/user/build-config-imports/).

**Please remember to tag versions for [`<path>@<ref>`](https://docs.travis-ci.com/user/build-config-imports/#importing-specific-versions-of-configs) notation.**

*Usage example:*  

```plain
import: pi-hole/.github:/build-configs/core.yml@v1.0.0
```

Pull Requests can `import` any reference.
>The format of the import source is `<account>/<repository>:<path>@<ref>` in which `<ref>` can be any valid Git reference, such as a commit sha, branch name, or tag name.
