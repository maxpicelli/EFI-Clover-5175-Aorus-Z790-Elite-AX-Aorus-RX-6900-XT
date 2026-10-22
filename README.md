# EFI Clover 5175 - Aorus Z790 Elite AX + RX 6900 XT

EFI destinada ao hardware abaixo, com Clover r5175 (`a193364cc`). A pasta EFI e o `config.plist` foram atualizados a partir do backup local em outubro de 2026.

## Hardware de referência

- **Placa-mãe:** Gigabyte Aorus Z790 Elite AX, revisão 1.0
- **Processador:** Intel Core i9-13900K (Raptor Lake, 8 P-cores + 16 E-cores, 32 threads)
- **GPU:** Aorus Radeon RX 6900 XT, 16 GB GDDR6

## Conteúdo da EFI

- **ACPI:** 18 SSDTs e a tabela DMAR em `CLOVER/ACPI/patched`
- **Drivers UEFI:** ApfsDriverLoader, OpenRuntime e VBoxHfs
- **Kexts:** ACPIMonitor, AirPortUtility, AirportItlwm, AppleALC, BluetoothFileExchange, CpuTopologyRebuild, FakeSMC, FeatureUnlock, HibernationFixup, ITEIT87x, IntelCPUMonitor, Lilu, LucyRTL8125Ethernet, NVMeFix, NaviAudioFixup, NootRX, RTCMemoryFixup, RadeonMonitor, RestrictEvents, USBPorts e USBWakeFixup
- **Configuração:** `CLOVER/config.plist`, com parâmetros de boot, gráficos, ACPI e patches de kernel/kext

O `config.plist` contém uma entrada de patch com o procedimento `_apfs_filevault_allowed`, relacionada ao macOS Tahoe. Isso, por si só, não garante compatibilidade geral com Tahoe nem significa que o FileVault esteja desativado.

## SMBIOS e identificadores

O SMBIOS existente foi preservado nesta atualização. Não substitua nem remova os valores de SMBIOS, MLB, ROM ou UUID ao atualizar esta EFI. Para usar a EFI em outro computador, gere identificadores próprios para esse equipamento.

## Compatibilidade e uso

O projeto é destinado ao hardware de referência. Compatibilidade com uma versão específica do macOS depende também das versões dos kexts e do sistema instalado; faça testes e mantenha uma cópia de recuperação da EFI antes de atualizar.

1. Faça backup da EFI funcional antes de substituir arquivos.
2. Confira as configurações da BIOS para a placa-mãe e a versão instalada; elas não são definidas por esta pasta EFI.
3. Verifique os efeitos dos patches e a configuração do FileVault antes de usar criptografia.

Este projeto é fornecido para fins educacionais e sem garantia. A execução do macOS em hardware que não seja Apple pode violar os termos de serviço da Apple.

**Última atualização:** outubro de 2026
**Clover:** r5175 (`a193364cc`)
