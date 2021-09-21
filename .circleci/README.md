# Orb Development Pipeline

This configuration file uses [orb-tools orb]() version 10 to automatically _pack_, _test_, and _publish_ CircleCI orbs using this project structure. View the comments within the config file for a full break  down

## Overview:

Release dev version of orb, for testing & possible publishing.

The `orb` will be published as `dev:alpha` and `dev:${CIRCLE_SHA1:0:7}`.
It requires a CircleCI API token to be stored as `CIRCLE_TOKEN` (default)
 https://circleci.com/docs/2.0/managing-api-tokens

Store the `CIRCLE_TOKEN` as a project env var or Contexts resource;
If using Contexts, add your context below.