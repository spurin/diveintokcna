# Dive Into Cloud Native, Containers, Kubernetes and the Kubernetes and Cloud Native Associate Certification - GCP Cloud Shell - Tutorial

![DiveInto](https://raw.githubusercontent.com/spurin/diveintokcna/cloudshell/DiveIntoKCNA_Cover.png)

This tutorial provides you with a fully working Kubernetes lab, accessible in your browser 🚀

Execute the following command to setup the lab environment.

For convenience you can send this to the terminal using the convenient 'Copy to Cloud Shell' icon on the top right of the text box

```bash
bin/docker-compose up -d
```

When this completes, you'll see text similar to the following -

```terminal
[+] Running 15/15
 ✔ Network kcna.diveinto.io                        Created                                                                                           0.1s 
 ✔ Network diveintokcna_default                    Created                                                                                           0.1s 
 ✔ Volume "diveintokcna_guest_home_control-plane"  Created                                                                                           0.0s 
 ✔ Volume "diveintokcna_root_home_control-plane"   Created                                                                                           0.0s 
 ✔ Volume "diveintokcna_shared"                    Created                                                                                           0.0s 
 ✔ Volume "diveintokcna_guest_home_worker-1"       Created                                                                                           0.0s 
 ✔ Volume "diveintokcna_root_home_worker-1"        Created                                                                                           0.0s 
 ✔ Volume "diveintokcna_guest_home_worker-2"       Created                                                                                           0.0s 
 ✔ Volume "diveintokcna_root_home_worker-2"        Created                                                                                           0.0s 
 ✔ Volume "diveintokcna_config"                    Created                                                                                           0.0s 
 ✔ Container shared-ssh-keys-dive-into-kcna        Exited                                                                                            4.4s 
 ✔ Container worker-2-dive-into-kcna               Started                                                                                           2.5s 
 ✔ Container worker-1-dive-into-kcna               Started                                                                                           2.4s 
 ✔ Container control-plane-dive-into-kcna          Started                                                                                           2.4s 
 ✔ Container portal-dive-into-kcna                 Started                                                                                           3.0s 
```

🚨 Important Step! - Must Be Completed Every Time 🚨

This step must be completed each time the lab environment is set up. The lab environment uses a Reverse Proxy to access Kubernetes web services. Occasionally, this may require permitting access from Google Cloud Shell.

To confirm accessibility, run the following command to generate your URL endpoint. After running the command, click the generated URL. You may be prompted to sign in. Once done, you should see the DiveInto Reverse Proxy with a blue background. After confirming, you can close the tab and continue.

```bash
echo https://32536-$WEB_HOST/testproxy
```

With the proxy running we can now access the Portal, click the Web Preview Icon, if you cant find it, click -> <walkthrough-web-preview-icon>here</walkthrough-web-preview-icon> for a walkthrough on where to find it.

Select 'Preview on Port 8080' and you're good to go!  

When accessing terminals, the default credentials are root/root

Should you require, you can factory reset the environment with the following, your terminals will disconnect and reconnect -

```bash
bin/docker-compose down -v; bin/docker-compose up -d
```
