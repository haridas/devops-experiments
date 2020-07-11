# devops-experiments
Different devops process and tools experiments

# Login to pulumi state store 

The state store can be kept locally or we can use the pulumi cloud. The state
store keep the last run information and current state of infrastructure that we
setup for a given project.

```bash
pulumi login --cloud-url gs://pulumi-state-bucket

pulumi login --local
```

After login with gs storage, ensure the bucket is created, pulumi won't create
it for you !
