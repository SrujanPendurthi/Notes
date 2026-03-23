.asm file that ends 55 aa(or 0x55 0xaa in HEX)

```
jmp $

times 510-($-$$) db 0
db 0x55,0xaa
```
This is a bare minimum boot sector

`jmp $` points to your actual code
`db 0x55, 0xaa` is the bootable flag

`$$` - begiing of current section
(`$ -$$`) is current address - section start =  length of previous code

The reason this is bare minium is because it is missing these parts:
	BPB/Header - Needed for file system compatibility
	Bootloader Code - actual logic
	Disk Signature - Unique ID for the drive
	Partition Table - defines where partitions live

