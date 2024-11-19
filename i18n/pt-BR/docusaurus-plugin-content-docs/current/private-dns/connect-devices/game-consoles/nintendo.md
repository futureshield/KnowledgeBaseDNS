---
title: Nintendo
sidebar_position: 2
---

Os consoles de jogos não oferecem suporte a DNS criptografado, mas são ótimos para configurar o AdGuard DNS Público ou o AdGuard DNS Privado via um Endereço de IP vinculado.

É provável que o seu roteador ofereça suporte ao uso de servidores DNS criptografados, então você pode configurar o Private AdGuard DNS nele e conectar seu console de jogos sempre que precisar.

[Como configurar seu roteador](/private-dns/connect-devices/routers/routers.md)

:::note Compatibility

Aplica-se a: Novo Nintendo 3DS, Novo Nintendo 3DS XL, Novo Nintendo 2DS XL, Nintendo 3DS, Nintendo 3DS XL e Nintendo 2DS.

:::

## Conectar o AdGuard DNS

Configure o seu console de jogos para usar um servidor público AdGuard DNS ou configure-o via IP vinculado:

1. No menu inicial, selecione _Configurações do sistema_.
2. Vá para _Configurações da Internet_ → _Configurações de conexão_.
3. Selecione o arquivo de conexão e selecione _Alterar configurações_.
4. Selecione _DNS_ → _Configurar_.
5. Defina _Obter DNS automaticamente_ como _Não_.
6. Selecione _Configurações Detalhadas_ → _DNS Primário_. Pressione a seta para a esquerda para excluir o DNS existente.
7. No campo _Servidor DNS_, insira um dos seguintes endereços de servidor DNS:
   - `94.140.14.49`
   - `94.140.14.59`
8. Salve as configurações.

Seria preferível usar o IP vinculado (ou o IP dedicado se você tiver uma assinatura Equipe):

- [IPs dedicados](/private-dns/connect-devices/other-options/dedicated-ip.md)
- [IPs vinculados](/private-dns/connect-devices/other-options/linked-ip.md)