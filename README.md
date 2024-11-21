## Tagging Strategy
In this workflow:

The image is always tagged with latest to represent the most up-to-date version.
Additionally, the image is tagged with the commit SHA (${{ github.sha }}), which is a unique identifier for each commit. This allows users to reference specific versions of the image for reproducibility and debugging.
For example, after a push to main, your Docker Hub repository will have images tagged:

## latest
## <commit-sha> (a unique tag for each commit)
 ## This dual-tagging strategy ensures that:

The latest stable version is easily accessible using the latest tag.
Older versions are still available using their commit-specific tags, which allows the team to reproduce a specific version if needed.
