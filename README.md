# This file helps you to setup MySql server in google cloud with Skaffold

Example YAML files for MySQL deployment using a StatefulSet on Google Cloud with Kubernetes self-manage.

### At first make sure that you have created a Persistent Disk in your Google Cloud project with the name (mysql-pd in this case)

```
gcloud compute disks create --size=10GB --zone=us-central1-c mysql-pd

```


# requirement 
1. Docker desktop install with kubernetes enable
2. Skaffold install on your desktop
3. Google Cloud SDK install in your desktop
4. Should has PersistentVolume, PersistentVolumeClaim, and mysql deployment yml file

### run this command in your terminal
```
skaffold dev

```