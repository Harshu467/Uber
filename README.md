# Build and deploy

Command to build the application. PLease remeber to change the project name and application name
```
gcloud builds submit --tag gcr.io/<ProjectName>/<AppName>  --project=<ProjectName>

gcloud builds submit --tag gcr.io/uber-366317/uber  --project=uber-366317
```

Command to deploy the application
```
gcloud run deploy --image gcr.io/<ProjectName>/<AppName> --platform managed  --project=<ProjectName> --allow-unauthenticated

gcloud run deploy --image gcr.io/uber-366317/uber --platform managed  --project=uber--allow-unauthenticated
```
