# RTL8723DS_BT_Linux

rtl8723ds default settings:
H5 protocol
Flow Control on
parity even
internal 32k clock

Host cts need connected to ground

sudo apt-get update
sudo apt-get upgrade
sudo apt-get install bluetooth blueman bluez bluez-tools rfkill libbluetooth-dev

sudo vi /etc/modules
add hci_uart in last line
reboot

lsmod | grep hci_uart

sudo make install
sudo rtk_hciattach -n -s 115200 ttyUSB0 rtk_h5

#you can change ttyUSB0 set-up depends on different requirements




