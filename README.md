# informatica_VM_cloud

Detailed Informatica requirements [here](https://docs.informatica.com/integration-cloud/cloud-platform/h2l/1382-how-to--install-and-configure-informatica-intelligent-cloud/install-and-configure-informatica-intelligent-cloud-services-in-/supported-configurations.html)  

Create VM for informatica
```
gcloud compute instances create instance-1 --project=tenacious-post-355715 --zone=us-central1-a --machine-type=n1-standard-4 --network-interface=network-tier=PREMIUM,subnet=default --maintenance-policy=MIGRATE --provisioning-model=STANDARD --service-account=1086204999159-compute@developer.gserviceaccount.com --scopes=https://www.googleapis.com/auth/devstorage.read_only,https://www.googleapis.com/auth/logging.write,https://www.googleapis.com/auth/monitoring.write,https://www.googleapis.com/auth/servicecontrol,https://www.googleapis.com/auth/service.management.readonly,https://www.googleapis.com/auth/trace.append --create-disk=auto-delete=yes,boot=yes,device-name=instance-1,image=projects/rhel-cloud/global/images/rhel-7-v20220519,mode=rw,size=20,type=projects/tenacious-post-355715/zones/us-central1-a/diskTypes/pd-balanced --no-shielded-secure-boot --shielded-vtpm --shielded-integrity-monitoring --reservation-affinity=any
```
