# INFO
`esptool.py -p /dev/cu.usbserial-0001 flash_id`

```txt
Detected flash size: 16MB
```

# READ
`esptool.py -p /dev/cu.usbserial-0001 read_flash 0x0 0x1600000 ./esp32.bin`


# WRITE
`esptool.py --baud 115200 -p /dev/cu.usbserial-0001 write_flash 0x0 ./esp32.bin`
