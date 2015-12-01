
##Cài đặt OpenVPN site- to- site trên Pfsense

### Mô hình triển khai:

<img src ="http://i.imgur.com/0rQ5vzB.png">

### Yêu cầu:
-	2 máy cài đặt pfsense.
-	2 máy client kết nối với hai máy Pfsense.

### Cài đặt:

####Site A (pfsense0)

Cấu hình trên site A với vai trò như một server

<img src="http://i.imgur.com/JsSPA0z.png">

**Chú ý:** Server mode chọn **Peer to Peer (Shared Key)**

<img src="http://i.imgur.com/EcZSdG8.png">
<img src="http://i.imgur.com/Nsw4561.png">

Sau đó các bạn chon **save**

<img src="http://i.imgur.com/MMzkjZq.png ">

Sau đó chọn edit -> copy Shared Key sang site B với vai trò như một client.
<img src ="http://i.imgur.com/SZwEeNg.png ">

Tạo rule trong WAN

<img src ="http://i.imgur.com/G0gDUuE.png ">
<img src ="http://i.imgur.com/mt7KmE7.png">

Tạo rule trong OpenVPN

<img src ="http://i.imgur.com/7raFwJf.png ">
<img src ="http://i.imgur.com/EcK4Wu8.png ">

####Site B (Pfsense1)

<img src ="http://i.imgur.com/ZiZxFrm.png">

**Chú ý:** Shared Key bỏ tích và copy Shared Key từ site A sang.

<img src ="http://i.imgur.com/fTGCwuq.png">
<img src ="http://i.imgur.com/qujiDea.png ">


Kết quả như hình dưới là bạn đã cấu hình thành công:

Site A
<img src ="http://i.imgur.com/QvRg2Kl.png">

Site B
<img src="http://i.imgur.com/QOTLmcc.png">













 
