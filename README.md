# Personalização do i3wm, i3blocks e Neofetch

Este repositório contém meus arquivos de configuração para o **i3wm**, **i3blocks** e **Neofetch**. O objetivo dessas personalizações é criar um ambiente minimalista, funcional e esteticamente agradável.

## i3wm - Gerenciador de Janelas

📁 **Local do arquivo:** `~/.config/i3/config`

O arquivo de configuração do i3wm é baseado no padrão, com ajustes pessoais para melhorar a usabilidade. As principais modificações incluem:
- Alterei algumas teclas de atalho para melhor fluxo de trabalho.
- Defini um layout padrão para as janelas.
- Configurei aplicações para abrir automaticamente ao iniciar o i3.
- Ajustei o comportamento de foco e movimentação de janelas.

Para aplicar as mudanças após edição:
```sh
mod+Shift+R  # Reinicia o i3wm sem deslogar
```

---

## i3blocks - Barra de Status

📁 **Local do arquivo:** `~/.config/i3blocks/config`

A configuração do **i3blocks** foi ajustada para incluir informações essenciais na barra de status, como:
- Uso da CPU e Memória
- Volume e brilho da tela
- Estado do Wi-Fi e Bluetooth
- Relógio e data

Para garantir que as alterações sejam aplicadas, reinicie a barra de status com:
```sh
pkill -SIGUSR1 i3blocks
```

Caso queira editar os scripts que fornecem os dados para os blocos, eles estão localizados em:
```sh
~/.config/i3blocks/scripts/
```

---

## Neofetch - Informações do Sistema

📁 **Local do arquivo:** `~/.config/neofetch/config.conf`

Modifiquei o Neofetch para:
- Exibir o logo da Apple em vez do sistema operacional padrão.
- Ajustar o layout da saída para melhor legibilidade.
- Alterar as cores do texto para combinar com o esquema visual do sistema.

Para testar sua configuração, basta rodar:
```sh
neofetch
```

---

## Como Instalar e Usar as Configurações
Caso queira utilizar estas configurações em seu ambiente, copie os arquivos para os diretórios correspondentes e reinicie o i3:
```sh
mkdir -p ~/.config/i3 ~/.config/i3blocks ~/.config/neofetch
cp i3/config ~/.config/i3/
cp i3blocks/config ~/.config/i3blocks/
cp neofetch/config.conf ~/.config/neofetch/
mod+Shift+R  # Reinicia o i3wm
```

Sinta-se à vontade para modificar os arquivos conforme suas necessidades! 🚀

