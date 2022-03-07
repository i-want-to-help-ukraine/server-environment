# Server environment

## Obtain personal access token
https://github.com/settings/tokens

## Docker login
* `$ export CR_PAT=YOUR_TOKEN`
* `$ echo $CR_PAT | docker login ghcr.io -u i-want-to-help-ukraine --password-stdin`

## npm login
` $ npm login --scope=@OWNER --registry=https://npm.pkg.github.com`\
`> Username: USERNAME`\
`> Password: TOKEN`\
`> Email: PUBLIC-EMAIL-ADDRESS`

## Staging

### Pre-requirement
* Docker login

### Start server
* `$ cd staging/`
* `$ docker-compose up -d`

### Shutdown server
* `$ cd staging/`
* `$ docker-compose down`
