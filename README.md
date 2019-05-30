# Introduction

This project illustrates the creation of a custom Spack release environment

# Use

To use this project, go to your Spack mirror on gitlab and in the CI settings add some environment variables:

```
SPACK_RELEASE_ENVIRONMENT_REPO = https://github.com/scottwittenburg/site-specific-release.git
SPACK_RELEASE_ENVIRONMENT_PATH = release_environment
```

The first variable tells Spack's `generate-gitlab-ci-yaml.sh` script to clone this repo to find the release environment, while the second tells that script the relative path within the repo to find the `spack.yaml` environment file.
