### Difference between tilde and caret in npm's package.json

Given a version number `major.minor.patch`

    ~major.minor.patch will allow patch-level changes
    ^major.minor.patch will allow minor- and patch-level changes (or more accurately, allow changes that don't modify the left-most non-zero digit)

<https://docs.npmjs.com/misc/semver#tilde-ranges-123-12-1>  
<http://bytearcher.com/articles/semver-explained-why-theres-a-caret-in-my-package-json/>
