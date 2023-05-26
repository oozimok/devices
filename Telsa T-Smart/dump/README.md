# INFO
`esptool.py -p /dev/cu.usbserial-0001 flash_id`

```txt
Detecting chip type... Unsupported detection protocol, switching and trying again...
Connecting...
Detecting chip type... ESP8266
Chip is ESP8266EX
Features: WiFi
Crystal is 26MHz
MAC: 80:64:6f:9f:de:9f
Uploading stub...
Running stub...
Stub running...
Manufacturer: a1
Device: 4015
Detected flash size: 2MB
```

# READ
`esptool.py -p /dev/cu.usbserial-0001 read_flash 0x0 0x200000 ./esp8266.bin`


# WRITE
`esptool.py --baud 115200 -p /dev/cu.usbserial-0001 write_flash 0x0 ./esp8266.bin`
