# Wifi - VLESS Server Configuration

This repository contains VLESS server configurations for Happ WiFi.

## Files

- **vless-servers.txt** - Plain text format with VLESS URIs (one per line)
- **vless-servers.json** - JSON format with detailed server information

## Import to Happ

### Using vless-servers.txt
Copy this raw URL into your Happ import:
```
https://raw.githubusercontent.com/geniitopik-create/Wifi/main/vless-servers.txt
```

### Using vless-servers.json
Copy this raw URL into your Happ import:
```
https://raw.githubusercontent.com/geniitopik-create/Wifi/main/vless-servers.json
```

## Server Details

Replace the example servers with your actual VLESS server information:
- **Server Address** - Your VPS/server IP or domain
- **Port** - VLESS port (typically 443, 8443, etc.)
- **UUID** - Your VLESS user UUID
- **SNI** - Server Name Indication (usually same as address)

## VLESS URI Format

```
vless://[UUID]@[ADDRESS]:[PORT]?encryption=[ENCRYPTION]&security=[SECURITY]&sni=[SNI]#[NAME]
```

**Parameters:**
- `encryption` - none (most common)
- `security` - tls, reality, or none
- `sni` - domain name for TLS
