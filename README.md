# JCasc Configurations for Jenkins
- We create this configuration as code used by Jenkins, were we defined some variables, global configurationa and also every credential used by Jenkins Pipelines.

## Globals configuration
- It is defined on this file as global configuration the way as connect to Gitlab and wish token must to use it.

## Variables configuration
- All variables defined on jenkins.yaml will be use by any Pipeline.

## Credentials configuration

- As we mention, all credentials that we need on Jenkins must to be defined at jenkins.yaml, keep in mind, that you need to encode any credential using base64, and also add to the secret: credentials-secret on Kubernetes.

Note: By the record, you will need call first at jenkins secret/value editing jenkins-value.yaml an then reload the configuration.

## Next steps
- Automate this implementation.
