# Sample Synthetic Populations

This repository contains definitions for sample synthetic populations which can be produced by [Synthea™](https://github.com/synthetichealth/synthea)

## Instructions
*These instructions assume you already have an up-to-date version of Synthea and all prerequisites installed and ready to run, and use `run_synthea` as the base command to run*
1. Download `module_overrides.properties` from a subfolder of this project to your local system
2. Switch Synthea to the `module_overrides` branch (required until this PR is merged: https://github.com/synthetichealth/synthea/pull/566 )
3. Run Synthea, specifying the downloaded `module_overrides.properties` as well as any other desired options:
```shell
> ./run_synthea --module_override=(path_to_module_overrides.properties)
```

For example, to generate 1,000 patients within the state of New York :

```shell
> ./run_synthea -p 1000 --module_override=(path_to_module_overrides.properties) "New York"

```

## License

Copyright 2019 The MITRE Corporation

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.
