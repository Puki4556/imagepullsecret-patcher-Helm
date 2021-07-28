# imagepullsecret-patcher-Helm
Helm chart for https://github.com/titansoft-pte-ltd/imagepullsecret-patcher

## Guide
1. Change the base64 string in vlaues.yaml.
2. helm install pullsecret-patcher .\pullsecret-patcher --namespace pullsecret-patcher --create-namespace

Base64 string example:
{"auths":{"https://index.docker.io/v1/":{"auth":"Base64_of_your_credentials"}},"credsStore":"ecr-login"}
Base64_of_your_credentials = UserName:Password
   
   
