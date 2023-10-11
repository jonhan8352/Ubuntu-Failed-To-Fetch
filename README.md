# Ubuntu-Failed-To-Fetch

We might experiencing failed to update our Ubuntu. This might be due to improper configuration during the Ubuntu Setup stage.

1. You will be receiving error when performing 'sudo apt update' or fail to install any package.
<img src="https://github.com/jonhan8352/Ubuntu-Failed-To-Fetch/blob/main/failed-to-fetech01.png">

2. You need to perform follow command to fix the nameserver (DNS) issue.
```
echo "nameserver 8.8.8.8" | sudo tee /etc/resolv.conf > /dev/null
```
3. Now try to update and upgrade your Ubuntu and packages.
```
sudo apt-get update
```
```
sudo apt-get upgrade
```
You're done!
