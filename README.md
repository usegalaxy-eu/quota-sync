# Galaxy-Google Response Quota Sync

Write a configuration file:

```yaml
url: https://usegalaxy.eu
key: ....
filename: 'Quota Request Form (Responses).tsv'
```

Then you can run it like:

```
BEARER_TOKEN_FILE=serviceaccounttoken.json GOOGLE_DRIVE_FILE_ID=<you can get the id from the files url> FILE_NAME='Quota Request Form (Responses).tsv' python download.py
CONFIG_FILE=conf.yaml python process.py
```

It will automatically generate missing quotas and synchronize the user list.

## LICENSE

GPLv3
