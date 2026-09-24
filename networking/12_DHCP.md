DHCP (Dynamic Host Configuration Protocol) არის პროტოკოლი, რომელიც მოწყობილობას ქსელში ჩართვისას ავტომატურად აძლევს ქსელურ პარამეტრებს.

მაგალითად, კომპიუტერი DHCP-ისგან იღებს:

IP Address
Subnet Mask
Default Gateway
DNS Server

ანუ ხელით შეყვანა აღარ არის საჭირო.

მოკლედ:
DHCP = მოწყობილობის ქსელის ავტომატური კონფიგურაციაა


    DHCP-ის მუშაობის ეტაპები — DORA

DHCP-ის დროს მოწყობილობასა და DHCP Server-ს შორის ხდება 4 ძირითადი ეტაპი:

Discover — კომპიუტერი ეძებს DHCP Server-ს.
Offer — DHCP Server სთავაზობს IP მისამართსა და სხვა ქსელურ პარამეტრებს.
Request — კომპიუტერი ითხოვს შეთავაზებულ კონფიგურაციას.
ACK (Acknowledgment) — DHCP Server ადასტურებს და კომპიუტერი იღებს პარამეტრებს.

მოკლედ:
Discover → Offer → Request → ACK

ამის შემდეგ კომპიუტერს უკვე აქვს IP, Subnet Mask, Gateway და DNS და შეუძლია ქსელში მუშაობა.