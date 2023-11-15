You only need to care about two files in each folder:
1. `sbom.json`: actual SBOM generated for the project and commit hash.
2. `result.json`: comparison result between the SBOM and maven dependency tree.
    - true positive: the dependency is in the SBOM and the dependency tree.
    - false positive: the dependency is in the SBOM but not in the dependency tree.
    - false negative: the dependency is not in the SBOM but in the dependency tree.
