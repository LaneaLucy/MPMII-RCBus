

all: bin ldr

ldr: xmpmldr.com

bin: hbios-ldrbios.bin


hbios-ldrbios.bin: hbios-ldrbios.z80
	~/RomWBW/Tools/Linux/uz80as hbios-ldrbios.z80 hbios-ldrbios.bin hbios-ldrbios.lst
	
xmpmldr.com: hbios-ldrbios.bin
	cat mpmldr.bin hbios-ldrbios.bin > xmpmldr.com


clean:
	rm -f hbios-ldrbios.bin hbios-ldrbios.lst xmpmldr.com






