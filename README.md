# Cara-Tambah-Port-Status-OpenWrt
- Open File Manager etc/ edit file Board.json atau klik di sini http://192.168.1.1/tinyfm/tinyfm.php?p=etc&view=board.json
- Masukan interface-name sesuai modem yang digunakan ikuti contoh seperti di bawah
# Menggunakan Script Di Bawah Ini, Port Status Nya Muncul Semua Walau Modem Tidak Connet
```
"ports": ["eth0","eth1","eth2","usb0"],

```
# Jika Menggunakan Script Yang Di Bawah Ini Port Status Muncul Saat Modem Terdeteksi 
```
{
 "model": {
 "id": "amlogic,p212",
 "name": "Amlogic Meson GXL (S905X) P212 Development Board"
 },
 "network": {
 "lan": {
 "device": "eth0",
 "protocol": "static"
 },
 "wan": {
 "device": "eth1",
 "protocol": "dhcp"
 },
 "tethering1": {
 "device": "usb0",
 "protocol": "dhcp"
 },
 "wan2": {
 "device": "eth2",
 "protocol": "dhcp"
		}
	}
}
```
- Jika Sudah File Nya Seperti di bawah
```
{
	"model": {
		"id": "amlogic,p212",
		"name": "Amlogic Meson GXL (S905X) P212 Development Board"
	},
	"network": {
		"lan": {
			"ports": ["eth0","eth1","eth2","usb0","wwan0"],
			"protocol": "static"
		}
	}
}

```
