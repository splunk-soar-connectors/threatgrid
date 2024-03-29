[comment]: # " File: README.md"
[comment]: # "Copyright (c) 2016-2024 Splunk Inc."
[comment]: # "Licensed under the Apache License, Version 2.0 (the 'License');"
[comment]: # "you may not use this file except in compliance with the License."
[comment]: # "You may obtain a copy of the License at"
[comment]: # ""
[comment]: # "  http://www.apache.org/licenses/LICENSE-2.0"
[comment]: # ""
[comment]: # "Unless required by applicable law or agreed to in writing, software distributed under"
[comment]: # "the License is distributed on an 'AS IS' BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND,"
[comment]: # "either express or implied. See the License for the specific language governing permissions"
[comment]: # "and limitations under the License."
[comment]: # "SPLUNK CONFIDENTIAL - Use or disclosure of this material in whole or in part"
[comment]: # "without a valid written license from Splunk Inc. is PROHIBITED."
[comment]: # ""
## Backward compatibility

-   The value for the ' **vm** ' parameter in the ' **detonate file** ' action is dynamic, so that
    the dropdown is removed from it. The list of available VMs can change from the ThreatGrid side.
    Run the ' **list vms** ' action to get the valid values for the ' **vm** ' parameter.
-   Some action data paths have been added/updated. Hence, it is requested to the end-user to please
    update their existing playbooks by re-inserting | modifying | deleting the corresponding
    action blocks.

## Port Information

The app uses HTTP/ HTTPS protocol for communicating with the ThreatGrid server. Below are the
default ports used by Splunk SOAR.

| Service Name | Transport Protocol | Port |
|--------------|--------------------|------|
| http         | tcp                | 80   |
| https        | tcp                | 443  |
