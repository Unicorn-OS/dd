# dd
block size: https://serverfault.com/questions/650086/does-the-bs-option-in-dd-really-improve-the-speed

example:
```
# Decompress
gunzip -c chromebook_oak-aarch64-bookworm.img.gz | sudo dd status=progress of=/dev/sd$

# image
sudo dd status=progress bs=512 if=chromebook_kukui-aarch64-bookworm.img of=/dev/sd$
```

# Decompress
https://unix.stackexchange.com/questions/632267/how-to-uncompress-a-gzipped-partition-image-and-dd-it-directly-to-the-destinatio

`gunzip -c /mnt/bkp/sda2.img.gz | sudo dd status=progress of=/dev/sda$`

# progress
https://askubuntu.com/questions/215505/how-do-you-monitor-the-progress-of-dd
`dd if=/dev/urandom of=/dev/null status=progress`
