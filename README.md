# <img src="https://github.com/pip-services/pip-services/raw/master/design/Logo.png" alt="Pip.Services Logo" style="max-width:30%"> <br/> Workspace for Integration Pip.Services

This is a workspace for [Integration Pip.Services](https://github.com/pip-services-integration) 
implemented in 5 different languages: .NET, Java, Node.js, Go and Python.

The workspace enables build, test, and release across the following projects:

- **pip-services-workflowstates-node** - Workflow states microservice in Node.js
- **pip-clients-workflowstates-node** - Client to workflow states microservice in Node.js
- **pip-services-duplicates-node** - Duplicates microservice in Node.js
- **pip-clients-duplicates-node** - Client to duplicates microservice in Node.js
- **pip-services-mappings-node** - ID mappings microservice in Node.js
- **pip-clients-mappings-node** - Client to ID mappings microservice in Node.js
- **pip-services-changescopes-node** - Change scopes microservice in Node.js
- **pip-clients-changescopes-node** - Client to change scopes microservice in Node.js
- **pip-clients-tempblobs-node** - Client to temp blobs microservice in Node.js
- **pip-libs-worklows-node** - Workflow framework in Node.js

## Installation

- Install **pip-tasks-ps**, **pip-tasks-common-ps** and **pip-tasks-node-ps** Powershell modules, 
add them to **PSModulePath** and import into Powershell

- Clone this workspace to local disk
```bash
> git clone https://github.com/pip-services-ecommerce/pip-services-integration-ws.git
```

- Got to the workspace folder and clone component repositories
```bash
> piptask clone -workspace
```

## Usage

- Setting default workspace
```bash
> pipuse <Path to this workspace>
```

- Start and stop ecommerce services
```bash
> piptask start -component pip-services-workflowstates
> piptask stop -component pip-services-workflowstates
```

- Building all components
```bash
> piptask build -all
```

- Test all components
``` bash
> piptask test -all
```

- Check out changes from remote repository
```bash
> piptask pull -all
```

- Check in changes to remote repository
```bash
> piptask push -m <Changes comment> -all
```

## Acknowledgements

The Integration Pip.Services are created and maintained by **Sergey Seroukhov**
