# circleci-trigger-project-build-orb

[![CircleCI](https://circleci.com/gh/zzish/circleci-trigger-project-build-orb.svg?style=svg)](https://circleci.com/gh/zzish/circleci-trigger-project-build-orb) [![CircleCI Orb Version](https://img.shields.io/badge/endpoint.svg?url=https://badges.circleci.io/orb/zzish/circleci-trigger-project-build-orb)](https://circleci.com/orbs/registry/orb/zzish/circleci-trigger-project-build-orb) [![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/zzish/circleci-trigger-project-build-orb/master/LICENSE) [![CircleCI Community](https://img.shields.io/badge/community-CircleCI%20Discuss-343434.svg)](https://discuss.circleci.com/c/ecosystem/orbs)

A simple orb for triggering project builds

To use this orb, try:

```
version: 2.1
orbs:
    circleci-trigger-project-build-orb: zzish/circleci-trigger-project-build-orb@2.0.0
workflows:
    foo:
        jobs:
            - circleci-trigger-project-build-orb/trigger:
                    token: ${CIRCLECI_API_TOKEN}
                    organization: foo
                    project: bar
```

To get a circleci api token go to:
https://circleci.com/docs/2.0/managing-api-tokens/#creating-a-personal-api-token
