🍀 # EFI Clover 5175 - Aorus Z790 Elite AX + RX 6900 XT

## 📋 Especificações do Hardware

### 🖥️ **Placa Mãe**
- **Modelo**: Gigabyte Aorus Z790 Elite AX (rev. 1.0)
- **Chipset**: Intel Z790
- **Socket**: LGA 1700

### 🔧 **Processador**
- **Modelo**: Intel Core i9-13900K (Raptor Lake)
- **Cores**: 24 (8P + 16E)
- **Threads**: 32

### 🎮 **Placa de Vídeo**
- **Modelo**: AMD Radeon RX 6900 XT
- **Fabricante**: Aorus (Gigabyte)
- **VRAM**: 16GB GDDR6

## 🚀 **Compatibilidade macOS**

- **macOS Sequoia** (15.x)
- **macOS Sonoma** (14.x)
- **macOS Ventura** (13.x)

## 📦 **Kexts Incluídos**

- **Lilu.kext** - Framework base
- **AppleALC.kext** - Áudio
- **NootRX.kext** - Suporte AMD RX 6900 XT
- **LucyRTL8125Ethernet.kext** - Ethernet
- **itlwm.kext** - WiFi Intel
- E outros kexts essenciais

## ⚙️ **ACPI Patches**

17 SSDTs incluídos para otimização do sistema.

## 🔒 **FileVault Disable Patcher**

Esta EFI inclui o **FileVault Disable Patcher** configurado no `config.plist` com procedimento `_apfs_filevault_allowed` para macOS Tahoe.

## ⚠️ **Avisos Importantes**

1. **Backup**: Sempre faça backup da sua EFI atual
2. **Serial Numbers**: Gere novos serial numbers únicos
3. **SMBIOS**: Configure o SMBIOS adequado para seu hardware
4. **FileVault**: Está desabilitado - não use se precisar de criptografia

## 🔧 **Configurações BIOS **

- Secure Boot: Desabilitado
- Fast Boot: Desabilitado
- CSM: Desabilitado
- Resizable BAR: desativado
- XMP/DOCP: Habilitado (DDR5)

---

**⚠️ Disclaimer**: Este projeto é apenas para fins educacionais. O uso de macOS em hardware não-Apple pode violar os termos de serviço da Apple. Use por sua própria conta e risco.

**📅 Última Atualização**: Setembro 2026
**🔧 Versão Clover**: 5175
**💻 Hardware**: Aorus Z790 Elite AX + RX 6900 XT + i9-13900K
