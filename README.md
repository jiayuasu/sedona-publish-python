# sedona-publish-python
 
This repo is to publish Sedona Python to Pypi. Sedona Python has builds for different OSs.

The reason why it is not under Apache is that ASF does not have a straightforward and safe way to set up GitHub secret.

To publish:

1. Replace the `python` folder with the latest Sedona Python release and commit the change.
2. The GitHub action will check if it can build wheels and dists.
3. Once all checks pass, manually create a GitHub release. This will trigger the publish process and upload Sedona Python to pypi.

This repo usually only accepts commits from Sedona PMC. A Sedona PMC can be added as an collaborator of this repo.