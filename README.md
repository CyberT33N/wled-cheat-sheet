# wled-cheat-sheet






# Flash
- https://install.wled.me/







<br><br>
<br><br>
___
<br><br>
<br><br>



# FAQ

## Error

### failed to execute 'open' on 'serialport': failed to open serial port
- Is caused by missing permissions

Option 1
```
# Check current permission for your usb port
ls -l /dev/ttyUSB0

# Change to 666
sudo chmod 666 /dev/ttyUSB0

# Then flash

# Now change back to your default permission
sudo chmod 660 /dev/ttyUSB0
```

Option 2
```shell
sudo usermod -aG dialout $USER

# Then log in & out again
```
