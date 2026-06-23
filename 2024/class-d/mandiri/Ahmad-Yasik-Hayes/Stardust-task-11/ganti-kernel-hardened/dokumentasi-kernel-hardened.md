# Install kernel
pacman -S linux-hardened linux-hardened-headers

# Edit config
nvim /etc/mkinitcpio.conf
<img width="1293" height="60" alt="image" src="https://github.com/user-attachments/assets/b406741e-bda2-40cb-b00c-af36716aac12" />

# Edit preset
nvim /etc/mkinitcpio.d/linux-hardened.preset
<img width="823" height="517" alt="image" src="https://github.com/user-attachments/assets/6d166c46-b621-4637-a341-bc5b6827b8b8" />

# Generate initramfs
mkinitcpio -P

# Reboot
note: karena sekarang anda sudah memiliki 2 kernel ketika ingin memasuki ulang silahkan spam tombol backspace lalu pilih linux hardened agar sistem lebih aman
