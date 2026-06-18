# MRI Installer - Distribuição Oficial 🚀

Read this in: [🇺🇸 English](README.en.md) | [🇪🇸 Español](README.es.md)

O **MRI Installer** é a porta de entrada para o ecossistema **MRI Qbox Brasil**. Uma ferramenta profissional, resiliente e segura para automatizar a instalação do seu servidor FiveM.

[![GitHub release (latest by date)](https://img.shields.io/github/v/release/mri-Qbox-Brasil/mri_installer_download?style=for-the-badge&color=7289da)](https://github.com/mri-Qbox-Brasil/mri_installer_download/releases/latest)
[![Security - VirusTotal Verified](https://img.shields.io/badge/Security-VirusTotal%20Scan-blue?style=for-the-badge&logo=virustotal)](https://github.com/mri-Qbox-Brasil/mri_installer_download/releases/latest)

---

## ✨ Por que usar o MRI Installer?

Diferente de instaladores comuns, o MRI foi construído com foco em **estabilidade** e **segurança**:

- 🛡️ **Segurança Verificada**: Cada versão enviada para este repositório é automaticamente escaneada pelo **VirusTotal**. O link do relatório está disponível em cada release.
- 💾 **Instalação Resiliente (Resume)**: Caiu a internet ou o PC desligou? O instalador detecta onde parou e retoma o progresso automaticamente, sem corromper arquivos.
- 🗄️ **Banco de Dados Automático**: Não tem o MariaDB instalado? O software cuida disso pra você em background, com resiliência contra bloqueios do Windows (UAC). Já tem um banco? Aponte para qualquer host/porta existente e visualize a senha enquanto configura.
- 👑 **txAdmin Personalizado**: O instalador configura automaticamente o nome do seu servidor e o idioma no painel administrativo.
- 🌎 **Totalmente em Português**: Interface intuitiva e suporte completo ao nosso idioma (disponível também em Inglês e Espanhol).
- 🐧 **Suporte a Linux**: Binário nativo para servidores Linux com instalador de terminal interativo ou totalmente automatizado via flags.

## 🚀 Como Começar

### Windows (interface gráfica)

1. Vá até a aba [**Releases**](https://github.com/mri-Qbox-Brasil/mri_installer_download/releases/latest).
2. Baixe o arquivo `mri_installer.exe`.
3. Execute o instalador e siga os 7 passos guiados (Ambiente, Motor, Receita, Resumo, Deploy, Configuração e Dashboard).

### Linux (terminal / servidor headless)

1. Vá até a aba [**Releases**](https://github.com/mri-Qbox-Brasil/mri_installer_download/releases/latest).
2. Baixe o arquivo `mri_installer_linux`.
3. Dê permissão de execução e rode:

```bash
chmod +x mri_installer_linux

# Modo interativo (recomendado para iniciantes)
./mri_installer_linux

# Modo não-interativo (flags completas)
./mri_installer_linux \
  --install-path /opt/fivem/mri_qbox \
  --server-name "Meu Servidor" \
  --license-key "cfxk_..." \
  --db-pass "senha" \
  --install-mariadb
```

> [!NOTE]
> No modo interativo, o instalador mostra um **código de liberação** de 8 caracteres. Autorize rodando `/liberar <código>` no nosso Discord **ou** abrindo o link exibido — não precisa de navegador no servidor.

> [!TIP]
> **Dica de Segurança**: Certifique-se sempre de baixar o executável deste repositório oficial da organização **MRI Qbox Brasil**.

## 🛡️ Transparência e Segurança

Nós levamos a segurança da nossa comunidade a sério. Por isso, integramos nosso pipeline de publicação com a API do **VirusTotal**.

Você pode encontrar o selo de segurança e o link para o relatório técnico completo na descrição de cada versão lançada.

O instalador também **não embute nenhuma credencial**: a validação de acesso e o download das receitas acontecem nos nossos servidores, então inspecionar o binário não revela chaves nem segredos.

---

Desenvolvido com ❤️ pela equipe [MRI QBOX BRASIL](https://github.com/mri-qbox-brasil)
