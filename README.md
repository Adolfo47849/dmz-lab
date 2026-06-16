# dmz-lab — Laboratorio de DMZ con Cisco Packet Tracer

## Objetivo

Configurar una red segmentada en tres zonas (LAN, DMZ y red externa) utilizando un router Cisco ISR como firewall en Cisco Packet Tracer, aplicando NAT estático y ACLs para controlar el tráfico entre zonas.

## Contenido del repositorio

```
dmz-lab/
├── README.md
├── dmz-lab.pkt                          # Archivo de Packet Tracer
├── informe/
│   └── Informe_DMZ_Laboratorio.md       # Informe técnico completo
└── evidencias/
    ├── evidencia_01_topologia.png
    ├── evidencia_02_pings_gateway.png
    ├── evidencia_03_web_antes_acl.png
    ├── evidencia_04_web_external_post_acl.png
    ├── evidencia_05_ping_external_falla.png
    ├── evidencia_06_web_internal.png
    ├── evidencia_07_ping_dmz_falla.png
    └── evidencia_08_show_commands.png
```

## Resumen de la topología

| Zona            | Red            | Dispositivos      |
|-----------------|----------------|-------------------|
| LAN Interna     | 192.168.1.0/24 | PC_Internal       |
| DMZ             | 192.168.2.0/24 | Server-PT Web_DMZ |
| Red Externa     | 192.168.3.0/24 | PC_External       |
| Router/Firewall | —              | Router_FW (ISR)   |

## Tecnologías utilizadas

- Cisco Packet Tracer
- NAT estático (ip nat inside source static)
- ACLs extendidas (access-list 100, 101)
- Protocolo HTTP (servidor web en DMZ)
Laboratorio de DMZ con Cisco Packet Tracer
