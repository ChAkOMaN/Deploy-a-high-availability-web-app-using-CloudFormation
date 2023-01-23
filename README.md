# Deploy-a-high-availability-web-app-using-CloudFormation
Creating this project will give you the hands-on experience you need to confidently talk about infrastructure as code. We have chosen a realistic scenario where you will deploy a dummy application (a sample JavaScript or HTML file) to the Apache Web Server running on an EC2 instance.

### Architecture
![Udagram Architecture]https://github.com/ChAkOMaN/Deploy-a-high-availability-web-app-using-CloudFormation/blob/main/HighAvailabilityWebApp.png


### To manage the architecture, some schell scripts have been created located in the /scripts folder.

### To create the stacks use the following shell scripts:

```sh
./scripts/create.sh hawebappinfra network/hawebapp.yml network/hawebapp.json

./scripts/create.sh hawebappservers server/hawebappservers.yml server/hawebappservers.json
```

### To update the stacks use the following shell scripts:

```sh
./scripts/update.sh hawebappinfra network/hawebapp.yml network/hawebapp.json

./scripts/update.sh hawebappservers server/hawebappservers.yml server/hawebappservers.json
```

### To delete the stacks use the following shell scripts:

```sh
./scripts/delete.sh hawebappinfra

./scripts/delete.sh hawebappservers
```