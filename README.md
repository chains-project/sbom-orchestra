# The Chains SBOM Orchestra

The Chains SBOM Orchestra is a chamber ensemble playing different SBOM tools.

It first performed at SCORED 2023 in Copenhagen on Nov 26 2023.

## SCORED 2023 Performance

* Prelude: presentation of the orchestra / team and the project (@Benoit)
* Git clone of https://github.com/xwiki/xwiki-rendering (@Benoit)
* Demo of GitHub SBOM (@MartinWitt)
* Demo of cdxgen 1.5 on project X (@Frank)
* Demo of syft (@Eric)
* Demo of tool CycloneDX-maven-plugin on project X (@Aman)
* Demo of tool build-info-go on project X (@Yogya)
* Conclusion: credits  (@Martin M.)
- Audio mixing (@Musard)

![IMG_7034](https://github.com/monperrus/misc/assets/803666/3b060816-1262-4f39-8529-1849008b78b5)


## Data
You only need to care about two files in each folder:
1. `sbom.json`: actual SBOM generated for the project and commit hash.
2. `result.json`: comparison result between the SBOM and maven dependency tree.
    - true positive: the dependency is in the SBOM and the dependency tree.
    - false positive: the dependency is in the SBOM but not in the dependency tree.
    - false negative: the dependency is not in the SBOM but in the dependency tree.
