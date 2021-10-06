# Policy Awareness CI/CD Demo

Wouldn't it be great to know if you were going to run into policy or compliance issues before you've even merged your infrastructure code into the main branch? Troubleshooting deployment issues after a PR is completed and the code is merged can get messy.  This repository highlights how ARM templates can be validated with Azure Policy as part of a GitHub Action.

## GitHub Action Repository

The action can be found in [this GitHub repository](https://github.com/jrob5756/defaults-policyaware-action). In the future, this action could be published to the GitHub Marketplace but, we have referenced the repository directly for now.  This is a proof of concept afterall.

## GitHub Action Triggers

The `Check Policy` action will be [triggered](https://docs.github.com/en/actions/learn-github-actions/events-that-trigger-workflows) whenever a pull request is created.

## Status Checks

The main branch has [branch protection rule](https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/defining-the-mergeability-of-pull-requests/managing-a-branch-protection-rule) which requires the `Check Policy` action to be successfully completed before a pull request can be merged.

## Related Topics

If you're new to the template development, see:

- [Azure Resource Manager](https://docs.microsoft.com/en-us/azure/azure-resource-manager/)
- [Azure Policy](https://docs.microsoft.com/en-us/azure/governance/policy/overview)
- [GitHub Actions](https://docs.github.com/en/actions)

`Tags: Azure Policy, ARM templates`
