# comodo
api串接import requests
url = 'https://verdict.valkyrie.comodo.com/api/v1/file/query/<sha1>'
標頭 = {'X-Api-Key': '03cf8788-a6c6-44f0-b014-ab6f887395eb'}
params = {'sha1': 'sha1|sha256|md5'}
response = requests.request('GET', url, params=params, headers=headers)
print(response.text)
