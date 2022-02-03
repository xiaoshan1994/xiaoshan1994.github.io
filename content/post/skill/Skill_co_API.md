---
title: "How to pull data from an API using Python"
date: 2022-01-24T17:10:17+01:00
categories:
- Skill
- Coding
tags:
- Python
- API
thumbnailImage: https://i2.wp.com/www.learnsteps.com/wp-content/uploads/2017/12/apis.png?fit=722%2C449&ssl=1
thumbnailImagePosition: left
metaAlignment: left
Math: True
---
<!--more-->
{{< toc >}}
# Pull data from an API in Python – A detailed Guide!
https://www.askpython.com/python/examples/pull-data-from-an-api
## Example 1: Pulling data from an Open source COVID API
In this example, we would be connecting to an Open source COVID API just to extract and parse the json information in an customized manner.
1. Connect to an API
At first, we need to connect to an API and make a secure connection as shown below–
In this article, we have used the COVID19-India API to fetch the data of the cases from the state-wise list.
```
import requests
import json
response_API = requests.get('https://api.covid19india.org/state_district_wise.json')
#print(response_API.status_code)
```
As we are pulling the data from an API, we have used the get() function to get the information from the API.

2. Get the data from API
After making a healthy connection with the API, the next task is to pull the data from the API. Look at the below code!
```
data = response_API.text
```
The requests.get(api_path).text helps us pull the data from the mentioned API.

3. Parse the data into JSON format
Having extracted the data, its now the time to convert and decode the data into proper JSON format as shown below–
```
json.loads(data)
```
4. Extract the data and print it
The JSON format contains data into a key-value format which resembles a Python dict. Thus, we can pull out and print the data using the key values as shown–
```
parse_json['Andaman and Nicobar Islands']['districtData']['South Andaman']['active']
```
You can find the entire code below!
```
import requests
import json
response_API = requests.get('https://api.covid19india.org/state_district_wise.json')
#print(response_API.status_code)
data = response_API.text
parse_json = json.loads(data)
active_case = parse_json['Andaman and Nicobar Islands']['districtData']['South Andaman']['active']
print("Active cases in South Andaman:", active_case)
```
Output:
```
Active cases in South Andaman: 19
```
## Example 2: Pulling data from an Open Source GMAIL API
Now, let us connect and pull data from GMAIL API. This API represents the generic structure and information which we can fetch from the API.
So, let us begin!
Have a look at the below code!
Example:
```
import requests
import json
response_API = requests.get('https://gmail.googleapis.com/$discovery/rest?version=v1')
#print(response_API.status_code)
data = response_API.text
parse_json = json.loads(data)
info = parse_json['description']
print("Info about API:\n", info)
key = parse_json['parameters']['key']['description']
print("\nDescription about the key:\n",key)
```
Output:
```
Info about API:
 The Gmail API lets you view and manage Gmail mailbox data like threads, messages, and labels.

Description about the key:
 API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
```
Explanation:
1. At first, we have connected to the generic GMAIL API using the `get()`function.
2. After forming a healthy connection with the API, we get the data from the API using `response_object.text`
3. Now, we parse the data into JSON format using `json.loads()` function.
4. Finally, we extract the data from the JSON object such as the description of the API an the description of the key.
5. You can cross check the values by visiting the API link mentioned in the example.
