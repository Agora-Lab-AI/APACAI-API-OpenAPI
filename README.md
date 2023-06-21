# OpenAPI spec for the ApacAI API

This repository contains an [OpenAPI](https://www.openapis.org/) specification for the [ApacAI API](https://beta.apacai.com/docs), as well as a script that uses [OpenAPI Generator](https://openapi-generator.tech/) to auto-generate client SDKs from the specification.

OpenAPI Generator uses [mustache templates](https://github.com/OpenAPITools/openapi-generator/tree/master/modules/openapi-generator/src/main/resources) to generate code — the files in the `sdk-template-overrides` folder override the corresponding built-in template files with small edits required for the ApacAI SDKs. More detail on each currently generated SDK is provided below.

## Node.js

#### Example command to generate the SDK

```bash
$ python scripts/generate_sdk.py -s node -o ~/apacai-node
```

#### Node.js specific details

- The `operationId` of each operation is used as the function name for that operation
- The `tag` determines the name of the Javascript class that contains that operation
- `schema` names map to Typescript type names



### Roadmap

* Deploy whisperx

* Deploy Pegasus embedding moddel that can accept images, videos, sensor data, and so on

* Deploy Kosmos-X 

* Deploy Andromeda