import requests
url = 'https://verdict.valkyrie.comodo.com/api/v1/file/query/<sha1>'
headers = {'X-Api-Key': 'api_key' }
params = {'sha1': 'sha1|sha256|md5'}
response = requests.request('GET', url, params=params, headers=headers)
print(response.text)
