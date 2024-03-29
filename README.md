# newrelic CircleCI Orb [![CircleCI Build Status](https://circleci.com/gh/moraesdam/circleci-newrelic.svg?style=shield "CircleCI Build Status")](https://circleci.com/gh/moraesdam/circleci-newrelic) [![CircleCI Orb Version](https://img.shields.io/badge/endpoint.svg?url=https://badges.circleci.io/orb/moraesdam/newrelic)](https://circleci.com/orbs/registry/orb/moraesdam/newrelic) [![GitHub License](https://img.shields.io/badge/license-MIT-lightgrey.svg)](https://raw.githubusercontent.com/moraesdam/circleci-newrelic/master/LICENSE) [![CircleCI Community](https://img.shields.io/badge/community-CircleCI%20Discuss-343434.svg)](https://discuss.circleci.com/c/ecosystem/orbs)

Record deployments on New Relic from your CircleCI workflow.
Use either the New Relic Application name or ID to do it.

This orb was based on these other:
* [finetune/newrelic](https://circleci.com/orbs/registry/orb/finetune/newrelic)
* [aarani/newrelic](https://circleci.com/orbs/registry/orb/aanari/newrelic)


## Usage

Example use-cases are provided on the orb [registry page](https://circleci.com/orbs/registry/orb/moraesdam/newrelic#usage-examples). Source for these examples can be found within the `src/examples` directory.


## Resources

[CircleCI Orb Registry Page](https://circleci.com/orbs/registry/orb/moraesdam/newrelic) - The official registry page of this orb for all versions, executors, commands, and jobs described.  
[CircleCI Orb Docs](https://circleci.com/docs/2.0/orb-intro/#section=configuration) - Docs for using and creating CircleCI Orbs.  

### How To Contribute

We welcome [issues](https://github.com/moraesdam/circleci-newrelic/issues) to and [pull requests](https://github.com/moraesdam/circleci-newrelic/pulls) against this repository!

To publish a new production version:
* Create a PR to the `Alpha` branch with your changes. This will act as a "staging" branch.
* When ready to publish a new production version, create a PR from `Alpha` to `master`. The Git Subject should include `[semver:patch|minor|release|skip]` to indicate the type of release.
* On merge, the release will be published to the orb registry automatically.

For further questions/comments about this or other orbs, visit the Orb Category of [CircleCI Discuss](https://discuss.circleci.com/c/orbs).

### Publishing

As this orb is structured using [FYAML](https://github.com/CircleCI-Public/fyaml), follow these steps to get it published:
1. Pack its source into a single yaml file: 
```
circleci config pack src > /tmp/orb.yaml
```
2. Publish it:
```
circleci orb publish /tmp/orb.yaml moraesdam/newrelic@X.Y.Z
``` 