[K8 cluster]

Deploying a 3 tier webapplication on kubernetes cluster using the app_manifest.yaml file

Here we are building a application with the front end which will update the redis database, workernode will get the details from the redis put the data in postgresSQL. result-app will dispaly the final results of the updates.

kubectl apply -f app_manifest.yaml

[Prometheus Monitoring and exposing the app]

For this we need to install the Prometheus and expose the pods using the exporter pod. Post this, we need to create a service monitor to to poll the data for the prometheus console.

Please find the prometheus_pod_monitor.md file for the detailed instructions.


Please get docker images from https://github.com/dockersamples/example-voting-app

