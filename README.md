# googledriveToCli

---

## installation ubuntu

```
apt update
apt install rclone -y
```

## configure rclone
```
rclone config
```

## check rclone
```
rclone listremotes
```

## create folder and mount with rclone
```
mkdir directory
```
```
rclone mount (your name directory config): directory
```

# 24h online

## edit file rclone-mount.sh 
```
sudo nano /usr/local/bin/rclone-mount.sh
```

## edit daemon reload with file rclone-mount

```
sudo nano /etc/systemd/system/rclone-mount.service
```

## reload daemon and run
```
sudo systemctl daemon-reload
sudo systemctl enable rclone-mount.service
sudo systemctl start rclone-mount.service
```

# Note
```
chmod +x /etc/systemd/system/rclone-mount.service
chmod +x /usr/local/bin/rclone-mount.sh
chmod 777 (directory)
```






