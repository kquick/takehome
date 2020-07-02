# Concrete Deliverables

## Pipeline

A CI pipeline (`.github/workflows/ci.yml`) that:

- bootstraps the repo
  - You can change this repo however, including adding git submodules if desired.
- builds both pieces of code, including any odd hacky-workarounds
- runs tests for both pieces of code
  - `cabal test`
  - `npm run test:unit`

## Dockerfiles

Fill out the dockerfiles to copy the code in and build the project.
Multistage builds, caching, efficiency, etc., are not required considerations.

Modify the `docker build` command in `.github/workflows/build-docker.yml` to match the ones in the README.
(the readme `docker build` invocations are probably right but are untested)
