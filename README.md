# Emerging Threats API Command Line Query Tool
This tool implements all of the functions of the ET 1.0 API and provides access to these functions via a BASH script. 

### Requirements
* bash
* curl
* hexdump (for stdout ouput)
* xxd (for stdout ouput)

### Optional Tool
* jq - Will help processing JSON on the command line

# Configuration
Edit the et_api script and modify the following value:
```
declare -r API_AUTH="<enter_et_api_key_here>"
```
### Showing Usage for API Components
![et_command_line_options_main](https://user-images.githubusercontent.com/83429267/194113797-1d8511af-b939-4067-b6fc-274f3b608ce5.png)

### Showing usage for reputation categories
![et_command_line_options_categories](https://user-images.githubusercontent.com/83429267/194113852-9ab72fac-bc5d-49d8-a590-2adbea8d2297.png)

### Showing usage for domains
![et_command_line_options_domains](https://user-images.githubusercontent.com/83429267/194113904-d6d0eb08-f759-4d45-9877-700e75f8dbd3.png)

### Showing usage for IPs
![et_command_line_options_ip](https://user-images.githubusercontent.com/83429267/194113922-2b7e6e72-f947-4b1f-ba20-af78142aefb4.png)

### Showing usage for samples
![et_command_line_options_samples](https://user-images.githubusercontent.com/83429267/194113944-ef0bf5a0-315d-4ec5-9010-8f76091a7e88.png)

### Showing usage for SIDS
![et_command_line_options_sids](https://user-images.githubusercontent.com/83429267/194113973-035096fe-20b0-44b9-81ef-45ade7f9320b.png)

# Usage

The following is an example of how to pull reputation categories from ET API and formatting it pretty with jq (pretty json):
![et_command_line_options_query_categories](https://user-images.githubusercontent.com/83429267/194114411-8bc3ba0a-38ef-4e6c-952b-8b2be065c51b.png)

The following is an example of how to pull reputation categories from ET API and formatting it pretty with jq (list format):
![et_command_line_options_query_categories_jq](https://user-images.githubusercontent.com/83429267/194114454-422486a3-e5e9-45fd-9b18-fa1e8589c629.png)

Query IP Geo Location:
![et_command_line_options_query_ip_rep](https://user-images.githubusercontent.com/83429267/194114380-06880ba3-4fc5-4243-9711-ac830ed9f224.png)

# Revisions
03/27/2017 - Initial Release  
06/06/2020 - Fixed CURL rvalue issue  
08/30/2021 - Fixed CURL command return codes  
