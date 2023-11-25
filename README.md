# dd
block size: https://serverfault.com/questions/650086/does-the-bs-option-in-dd-really-improve-the-speed

example:
`sudo dd bs=512 if=chromebook_kukui-aarch64-bookworm.img of=/dev/sd$`

# Decompress
https://unix.stackexchange.com/questions/632267/how-to-uncompress-a-gzipped-partition-image-and-dd-it-directly-to-the-destinatio

`gunzip -c /mnt/bkp/sda2.img.gz | sudo dd of=/dev/sda$`
