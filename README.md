###🗈️ Gallery — CTF Challenge (Dockerlabs Edition) ###

Gallery is a vulnerable web-based CTF machine distributed through Dockerlabs.es. It is packaged in .tar format and deployed automatically using the provided auto_deploy.sh script.

##⚙️ Requirements ##

Docker

Sudo privileges

##📅 Download ##

You can download the .zip file containing the lab from Dockerlabs.es. After extracting it, you'll find:

gallery.tar → The Docker image

auto_deploy.sh → Deployment script

## 🚀 How to Launch the Machine ##

✅ Recommended Method (Auto Deploy)

```
sudo bash auto_deploy.sh gallery.tar
```

This will automatically deploy the vulnerable machine and display its assigned IP address.

Press Ctrl+C when you're done to stop and remove the container.

## 🔧 Manual Method (Optional) ##

```
docker load -i gallery.tar
docker images               # Locate the image name or ID
docker run -dit --rm <image_name_or_id>
```

The image includes a predefined entrypoint that configures services and exposes necessary ports.

## 🔍 Writeup ##

A full walkthrough is available here:
https://rsas-book.gitbook.io/rsas-book/projects/my-ctfs/galeria

⚠️ This link contains spoilers and should be opened **only after attempting the machine yourself.

❗ Legal Disclaimer

This machine is intentionally vulnerable and is meant to be used strictly in controlled environments for educational and ethical hacking purposes only.

## 📜 License ##

MIT License


