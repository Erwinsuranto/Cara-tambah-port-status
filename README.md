# Cara-Tambah-Port-Status-OpenWrt
- Open File Manager etc/ edit file Board.json
- Masukan interface-name sesuai modem yang digunakan ikuti contoh seperti di bawah
```
"ports": ["eth0","eth1","eth2","usb0"],

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
