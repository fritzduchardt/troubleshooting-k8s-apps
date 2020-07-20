# Solution

- In `job.yaml` the job calls "localhost" which can not get resolved. Change "localhost" to "theserver".
- The database configuration in `deployment.yaml` is invalid. Change "super-safe-passwd" in `postgres.yaml` to "password".