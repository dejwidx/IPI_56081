# VPN dla pracy zdalnej z WireGuard

Dokumentacja projektowa realizowana w ramach przedmiotu **Innowacyjny Projekt Indywidualny** (Uniwersytet DSW, semestr zimowy 2026/2027).

## 1. Opis problemu i cel projektu
Projekt rozwiązuje problem braku bezpiecznego i odizolowanego dostępu zdalnego do zasobów wewnętrznych małej firmy (serwer plików, intranet, ERP). Rozwiązanie zakłada wdrożenie bramki VPN opartej na protokole WireGuard z uwierzytelnianiem za pomocą par kluczy kryptograficznych oraz filtracją ruchu między podsieciami VLAN.

## 2. Stos technologiczny
- **Infrastruktura sieciowa:** OPNsense (Firewall / NAT / Port Forwarding UDP 51820), przełącznik zarządzalny L2 (802.1Q VLAN)
- **Usługi serwerowe:** Ubuntu Server 24.04 LTS (VirtualBox), WireGuard (`wg-quick`), `ufw`/`nftables`, WG-Easy (Docker)
- **Narzędzia projektowe:** Cisco Packet Tracer, Draw.io

## 3. Struktura repozytorium
- `/docs` – dokumentacja opisowa projektu (wersje robocze oraz finalny plik PDF)
- `/diagrams` – schemat architektury systemu oraz topologia sieciowa
- `/configs` – przykładowe pliki konfiguracyjne (`wg0.conf`, skrypty Bash/Python, plik `.pkt` z Cisco Packet Tracer)

## 4. Kamienie milowe
- [x] Wybór tematu, zdefiniowanie stosu technologicznego i zakresu MoSCOW
- [ ] Konsultacje: koncepcja, architektura, harmonogram Gantta i analiza ryzyka (22.11.2026)
- [ ] Finalizacja dokumentacji PDF oraz diagramów w repozytorium (24.01.2027)
