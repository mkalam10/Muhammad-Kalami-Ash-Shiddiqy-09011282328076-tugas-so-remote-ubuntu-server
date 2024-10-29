# Muhammad-Kalami-Ash-Shiddiqy-09011282328076-tugas-so-remote-ubuntu-server
Langkah langkah untuk remote linux server dengan linux desktop: 
1. download file iso ubuntu server dari web resmiya
2. install ubuntu server di virtual box ( gunakan bridge adapter )
3. install ssh di ubuntu server dengan perintah sudo apt install openssh-server dan ubah port ke 40 dengan perintah sudo nano /etc/ssh/sshd_config
4. izinkann port baru di firewall dengan perintah sudo ufw allow 40/tcp
5. restart ubuntu server dengan sudo systemctl restart ssh dan cek apakah portnya sudah berubah ( gunakan sudo systemctl status ssh )
6. lihat ip address dengan perintah ifconfig ( disini ip address saya adalah 192.168.100.217 )
7. kemudian masuk ke linux desktop 
8. gunakan perintah ssh kalam@192.168.100.217 -p 40 untuk masuk ke server 
9. atur agar user ip address serta port sesuai dengan yang di server
10. jika sudah sesuai semua login akun dari linux desktop dan masukkan password server nya 


