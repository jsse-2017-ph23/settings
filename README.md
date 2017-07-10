# settings
Settings files for various cloud services

The following sections assume [Firebase CLI] and [Google cloud SDK] are installed and set up.

[Firebase CLI]: https://firebase.google.com/docs/hosting/quickstart
[Google cloud SDK]: https://cloud.google.com/sdk/docs/

## Firebase realtime database security rules
Firebase database have some security rules to be deplyed for better security.
Run the following command to update security rule

```shell
firebase deploy --only database
```

__WARNING__: The rules are not guaranteed to be the latest. I may forget to update rules in this repo.

## Google cloud storage CORS settings
CORS need to be set up before web client can receive images from cloud storage.

```shell
gsutil cors set cors-json-file.json gs://jsse-2017.appspot.com
```
