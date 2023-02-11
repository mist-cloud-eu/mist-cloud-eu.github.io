#  mist-cloud -- Infraless compute cloud

## Mental model: Rapids-rivers
### The problem with monoliths
### The problem with direct communication
### The problem with front-end first
### The problem with always-on
### The problem with cold starts
### The problem with single tier message queues
### The solution
## Running code: Different event flows (Local simulator)
### Getting set up
### Request-response 1: Simple server-client
### Micro front-end
### Request-response 2: Server-client with extra steps
### Request-response 3: Inter-service communication
### Streaming front-end
## Going cloud: Adding data (cloud)
### Getting set up
#### Early Access
#### Roles
#### API Keys
#### Deployment
#### Secrets
##### Database: Elephant SQL
### Splitting and merging
### Rendezvous
## Going professional: Automated safety
### Getting set up
#### Git hosting: Gitlab
### Continuous integration
#### Service testing
#### Static analyses
### Continuous deployment
#### Deploy to mist-cloud
#### Smoke test
## Going big: Typed events
### Getting set up
#### Gitlab package registry
#### Protobuf
### Using the event registry
### Automatic packages for multiple languages
## Building for scale
### Idempotence
### Backup



