# Mangled Migration 

## Installation
```
kubectl apply -f problems/jobs/mangled-migration/
```

## Description

The user wants to run a data migration. For this purpose he wants to run a job that calls an internal endpoint on hist application. This will trigger the data migration on the application Pod. 

For some reason the job does not complete successfully.

## Expected result

The job should run successfully.