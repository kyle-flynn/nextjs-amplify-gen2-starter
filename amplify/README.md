# Application Back-End Infrastructure

## Sandbox Amplify Environment for Local Development

### Create a Local AWS Profile

`aws configure --profile <PROFILE_NAME>`

The access key id and secret access key should be given via csv file.

Use `us-east-2` or `us-east-1` as the deployment region, and `json` as the output format.

You can export the default aws profile via `export AWS_PROFILE=<PROFILE_NAME>` or `$env:AWS_PROFILE="<PROFILE_NAME>"`

This aws account only has deploy permissions. This should be used for local development only.

### Deploying Amplify Sandbox

First install dependencies via `npm i`

Run `npx ampx sandbox --profile <PROFILE_NAME>` in the `/inrfa` directory.

Amplify will now synthesize and deploy the needed resources to aws.
