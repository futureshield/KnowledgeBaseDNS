---
title: Windows
sidebar_position: 5
---

For at tilslutte en iOS-enhed til AdGuard DNS, føj den først til _Kontrolpanel_:

1. Gå til _Kontrolpanel_ og klik på _Tilslut ny enhed_.
2. Vælg Windows i rullemenuen _Enhedstype_.
3. Navngiv enheden.
   ![Tilslutning af enhed \*mobile\_border](https://cdn.adtidy.org/content/kb/dns/private/new_dns/connect/windows_ab/choose_windows.png)

## Brug AdGuard Ad Blocker (betalt mulighed)

Med AdGuard-appen kan man bruge krypteret DNS, hvilket gør den perfekt til opsætning af AdGuard DNS på en Windows-enhed. Man kan vælge mellem forskellige krypteringsprotokoller. Sammen med DNS-filtrering får man også en fremragende adblocker, der fungerer på hele systemet.

1. [Installér appen](https://adguard.com/adguard-windows/overview.html) on the device you want to connect to AdGuard DNS.
2. Åbn appen.
3. Klik på _Indstillinger_ øverst på app-startskærmen.
   ![Indstillinger \*border](https://cdn.adtidy.org/content/kb/dns/private/new_dns/connect/windows_ab/windows_step3.png)
4. Vælg fanen _DNS-beskyttelse_ fra menuen til venstre.
   ![DNS-beskyttelse \*border](https://cdn.adtidy.org/content/kb/dns/private/new_dns/connect/windows_ab/windows_step4.png)
5. Klik på den aktuelt valgte DNS-server.
   ![DNS-server \*border](https://cdn.adtidy.org/content/kb/dns/private/new_dns/connect/windows_ab/windows_step5.png)
6. Rul ned og klik på _Tilføj en tilpasset DNS-server_.
   ![Tilføj en tilpasset DNS-server \*border](https://cdn.adtidy.org/content/kb/dns/private/new_dns/connect/windows_ab/windows_step6.png)
7. Indsæt i feltet DNS upstreams en af flg. adresser. Er man usikker på, hvilken én man skal vælge, vælg DNS-over-HTTPS.
   ![DoH-server \*border](https://cdn.adtidy.org/content/kb/dns/private/new_dns/connect/windows_ab/windows_step7_1.png)
   ![Opret server \*border](https://cdn.adtidy.org/content/kb/dns/private/new_dns/connect/windows_ab/windows_step7_2.png)
8. Tryk på _Gem og vælg_.
   ![Gem og vælg \*border](https://cdn.adtidy.org/content/kb/dns/private/new_dns/connect/windows_ab/windows_step8.png)
9. Den tilføjede DNS-server vises nederst på listen _Tilpassede DNS-servere_.
   ![Tilpassede DNS-servere \*border](https://cdn.adtidy.org/content/kb/dns/private/new_dns/connect/windows_ab/windows_step9.png)

Færdig! Enheden er nu tilsluttet AdGuard DNS.

## Brug af AdGuard VPN

Ikke alle VPN-tjenester understøtter krypteret DNS. Det understøttes dog af vores VPN, så har man behov for både et VPN og en privat DNS, er AdGuard VPN det oplagte valg.

1. Installér AdGuard VPN.
2. Åbn appen og klik på _Indstillinger_.
3. Vælg _App-indstillinger_.
   ![App-indstillinger \*border](https://cdn.adtidy.org/content/kb/dns/private/new_dns/connect/windows_vpn/windows_step4.png)
4. Rul ned og vælg _DNS-servere_.
   ![DNS-servere \*border](https://cdn.adtidy.org/content/kb/dns/private/new_dns/connect/windows_vpn/windows_step5.png)
5. Klik på _Tilføj tilpasset DNS-server_.
   ![Tilføj tilpasset DNS-server \*border](https://cdn.adtidy.org/content/kb/dns/private/new_dns/connect/windows_vpn/windows_step6.png)
6. Indsæt i feltet _Serveradresse_ en af flg. adresser. Er man usikker på, hvilken én man skal vælge, vælg DNS-over-HTTPS.
   ![DoH-server \*border](https://cdn.adtidy.org/content/kb/dns/private/new_dns/connect/windows_vpn/windows_step7_1.png)
   ![Opret server \*border](https://cdn.adtidy.org/content/kb/dns/private/new_dns/connect/windows_vpn/windows_step7_2.png)
7. Tryk på _Gem og vælg_.
   ![Gem og vælg \*border](https://cdn.adtidy.org/content/kb/dns/private/new_dns/connect/windows_vpn/windows_step8.png)

Færdig! Enheden er nu tilsluttet AdGuard DNS.

## Brug AdGuard DNS Client

AdGuard DNS Client er et alsidigt, tværplatforms konsolværktøj, der muliggør AdGuard DNS-tilslutning vha. krypterede DNS-protokoller.

Flere detaljer kan findes i [forskellig artikel](/dns-client/overview/).

## Opsæt almindelig DNS

Foretrækker man ikke at bruge ekstra software til DNS-opsætning, kan der vælges ikke-krypteret DNS. Man har to valg: Brug linkede IP'er eller dedikerede IP'er.

- [Dedikerede IP'er](/private-dns/connect-devices/other-options/dedicated-ip.md)
- [Linkede IP'er](/private-dns/connect-devices/other-options/linked-ip.md)