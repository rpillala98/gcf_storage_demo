# Cloud storage triggered Cloud Function demo

Sample that shows how to trigger a cloud function when a file is uploaded to cloud storage.

## deploy instructions
```
gcloud functions deploy storage_demo \
--runtime nodejs18 \
--entry-point fileData \
--trigger-event google.storage.object.finalize \
--trigger-resource sp24-cit50100-rpillala-demo-bucket
```

 