# 2 - Glosario Ciberseguridad (Conocimientos genéricos)

**Objetivo**: Leer y resumir glosario INCIBE esencial para transversales Cero/INCLUDE. Usar IA para reforzar comprensión.[file:1][file:2]

## Tabla 10 términos clave

| Término | Def oficial INCIBE | Explicación Bing/Copilot | Explicación GPT | Diferencias |
|---------|--------------------|---------------------------|-----------------|-------------|
| Ransomware | Programa malicioso que cifra archivos y exige rescate para descifrarlos. | Secuestra datos hasta pago; ejemplo 2025: LockBit ataca hospitales. Como dev Java, imagina endpoint cifrado en tu API. | Malware que bloquea acceso; usa cripto asimétrica. Ej: Ryuk en empresas 2025. Relación web: inyecciones via forms. | GPT más técnico (cripto); Bing práctico (ej real). |
| Phishing | Técnica para obtener datos sensibles haciéndose pasar por entidad confiable. | Emails falsos BancoX; 2025: campañas IA-generadas. En dev: valida siempre inputs user. | Suplantación identidad; vishing/spear. Ej: Google Docs 2025. Web dev: HTTPS + CSP. | GPT tipos variantes; Bing foco emails. |
| Firewall | Sistema que monitoriza tráfico y bloquea accesos no autorizados. | Guardia red; ej WAF Cloudflare. Java: Spring Security rules. | Filtro paquetes; stateful/NGFW. 2025: zero-trust models. | Bing ejemplo tool; GPT tipos avanzados. |
| Malware | Software malicioso diseñado para dañar/ robar info sin consentimiento. | Virus/troyanos; 2025: Android banking. Escanea con antivirus en builds. | Paraguas: spyware/adware/rootkits. Prevención: sandboxing code. | Similar; GPT más categorías. |
| Exploit | Código que aprovecha vulnerabilidad para ejecutar acciones no autorizadas. | CVE-2025-XXXX en Log4j-like; patcha deps Maven ya. | Input malicioso; zero-click iOS 2025. Dev: OWASP top10 checks. | Bing dev-relacionado; GPT mobile focus. |
| DDoS | Ataque que satura recursos impidiendo servicio legítimo. | Flood SYN; 2025: botnets IoT. Mitiga con CDN rate-limit. | Volumétrico/aplicación; Cloudflare Magic. Java: thread pools limits. | GPT capas ataque; Bing mitigación. |
| Encriptación | Proceso matemático para hacer datos ilegibles sin clave. | AES-256 HTTPS; usa BCrypt passwords Java. | Simétrica/asimétrica (RSA). 2025: quantum-resistant. | GPT algoritmos; Bing práctica dev. |
| VPN | Red privada virtual que cifra tráfico vía túnel seguro. | Acceso remoto seguro; ej NordVPN dev testing. | IPsec/WireGuard; oculta IP. 2025: post-cuanticos. | Bing uso dev; GPT protocolos. |
| Zero-day | Vulnerabilidad desconocida por vendor, explotada por atacantes. | Log4Shell inicial; monitora GitHub advisories. | Día cero patch; bounty programs. Ej: Chrome 2025. | GPT programas bounty; Bing monitoring. |
| MFA | Autenticación que requiere ≥2 factores (algo sabes/tienes/eres). | Google Auth + password; implementa en Spring Boot. | TOTP/HW keys; 2025: passkeys. | Bing código impl; GPT evol passkeys. |

## Reflexión
- **Más útil**: Ejemplos reales 2025 + relación con Java/web dev (inputs, deps, security).  
- **IA diferencia**: Bing más "práctico/dev-oriented"; GPT "teórico/técnico". Ambas confirman necesidad **siempre validar/sanitizar**.  
- Nivel confianza pre: 2/5 → post: 3.5/5.
- 
## Tiempo invertido
- Total: 120 minutos.
- Bloqueos: Ninguno 

**Recursos**: [Glosario INCIBE](https://www.incibe.es/sites/default/files/contenidos/guias/doc/guia_glosario_ciberseguridad_2021.pdf)
---

*Documentado por David Nuñez - Preparación curso IT/Ciberseguridad marzo 2026. Fundación GoodJob.*
