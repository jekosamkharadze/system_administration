TCP/IP მოდელი აღწერს, როგორ გადაადგილდება მონაცემი ერთი მოწყობილობიდან მეორემდე ქსელში.

ფენებია:

5. Application
4. Transport
3. Network
2. Data Link
1. Physical


1. Physical — ფიზიკური ფენა

აქ ხდება მონაცემის ბიტების ფიზიკური გადაცემა.

მაგალითად:

Ethernet კაბელი
ოპტიკური ბოჭკო
Wi-Fi რადიოსიგნალი
ელექტრული/ოპტიკური სიგნალი

Physical = როგორ გადადის 0 და 1 ფიზიკურად.

2. Data Link — მონაცემთა არხის ფენა

აქ მუშაობს ლოკალური ქსელის კომუნიკაცია.

მთავარი ელემენტებია:

MAC Address
Ethernet Frame
Switch

მაგალითად, Switch MAC Address-ის მიხედვით განსაზღვრავს, რომელ პორტზე უნდა გააგზავნოს Frame.

Data Link = MAC + Ethernet + Switch

3. Network — ქსელური ფენა

აქ მთავარი არის IP Address და Routing.

მთავარი ელემენტებია:

IP Address IPv4 / IPv6
Router
Routing

Router Destination IP-ის მიხედვით განსაზღვრავს, რომელი მიმართულებით უნდა წავიდეს პაკეტი.

Network = IP + Routing + Router

4. Transport — სატრანსპორტო ფენა

ეს ფენა უზრუნველყოფს მოწყობილობებს შორის მონაცემების ტრანსპორტირებას.

მთავარი პროტოკოლებია:

TCP
UDP

ასევე აქ გვხვდება Port, მაგალითად:

192.168.1.10:443

აქ 443 განსაზღვრავს კონკრეტულ ქსელურ სერვისს.

Transport = TCP/UDP + Port

5. Application — აპლიკაციის ფენა

ეს არის მომხმარებელთან და ქსელურ სერვისებთან ყველაზე ახლოს მყოფი ფენა.

აქ გვხვდება:

HTTP/HTTPS — ვებგვერდები
DNS — დომენის IP-ად გადაყვანა
DHCP — ქსელური პარამეტრების ავტომატურად მიღება
SSH — დისტანციური მართვა
FTP — ფაილების გადაცემა

Application = ქსელური სერვისები და მათი პროტოკოლები



მარტივად:
Application → HTTP, DNS, DHCP, SSH
Transport   → TCP, UDP, Port
Network     → IP, Router, Routing
Data Link   → MAC, Ethernet, Switch
Physical    → Cable, Signal, Wi-Fi

Physical — როგორ გადადის სიგნალი
Data Link — ვის მივაწოდოთ ლოკალურ ქსელში (MAC)
Network — რომელ ქსელში/მიმართულებით წავიდეს (IP)
Transport — რომელ სერვისს მიეწოდოს და როგორ გადაიცეს (TCP/UDP, Port)
Application — რა ქსელურ სერვისს ვიყენებთ (HTTP, DNS, DHCP და ა.შ.)