# Site-to-site-OpenVPN-on-Pfsense

#Cài đặt OpenVPN site- to- site trên Pfsense

### Mô hình triển khai:

http://i.imgur.com/0rQ5vzB.png

### Yêu cầu:
-	2 máy cài đặt pfsense.
-	2 máy client kết nối với hai máy Pfsense.

### Cài đặt:

####Site A (pfsense0)

Cấu hình trên site A với vai trò như một server

<img src="http://i.imgur.com/JsSPA0z.png">

Chú ý: Server mode chọn  Peer to Peer (Shared Key)
<img src = " ">
<img src = " ">
<img src = " ">
<img src = " ">
<img src = " ">
<img src = " ">
<img src = " ">
<img src = " "><img src = " ">
http://i.imgur.com/EcZSdG8.png
http://i.imgur.com/Nsw4561.png
Sau đó các bạn chon save
http://i.imgur.com/MMzkjZq.png

Sau đó chọn edit -> copy Shared Key sang site B với vai trò như một client.
http://i.imgur.com/SZwEeNg.png
Tạo rule trong WAN
http://i.imgur.com/G0gDUuE.png
http://i.imgur.com/mt7KmE7.png

Tạo rule trong OpenVPN
http://i.imgur.com/7raFwJf.png
http://i.imgur.com/EcK4Wu8.png
Site B (Pfsense1)
http://i.imgur.com/ZiZxFrm.png
Chú ý: Shared Key bỏ tích và copy Shared Key từ site A sang.
http://i.imgur.com/fTGCwuq.png
http://i.imgur.com/qujiDea.png

 
