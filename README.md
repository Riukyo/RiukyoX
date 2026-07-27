<div align="center">

<img src="https://raw.githubusercontent.com/Riukyo/RiukyoX/main/assets/Icone-Logo.svg" alt="RiukyoX Logo" width="110" />

# RiukyoX

**The Next-Generation Low-Latency Engine & System Optimizer for Windows**  
*O Ecossistema Definitivo de Latência e Performance para Windows*

[![Downloads](https://img.shields.io/github/downloads/Riukyo/RiukyoX/total?style=flat-square&color=7c3aed&logo=github)](https://github.com/Riukyo/RiukyoX/releases)
[![Version](https://img.shields.io/badge/version-1.0.7--beta-7c3aed?style=flat-square)](https://github.com/Riukyo/RiukyoX/releases)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011%20x64-0078D6?style=flat-square&logo=windows11&logoColor=white)](https://github.com/Riukyo/RiukyoX/releases)
[![Discord](https://img.shields.io/badge/Discord-Comunidade-5865F2?style=flat-square&logo=discord&logoColor=white)](#)

[📥 Download Direct (v1.0.7)](https://github.com/Riukyo/RiukyoX/releases/download/v1.0.7/riukyox-wizard.exe) &nbsp;•&nbsp; [📖 Release Notes](https://github.com/Riukyo/RiukyoX/releases) &nbsp;•&nbsp; [💬 Discord](#)

</div>

---

## Sobre o RiukyoX

O **RiukyoX** é uma plataforma de otimização de alta performance desenvolvida em **Rust** para remover gargalos de latência entre os comandos do jogador e a resposta na tela. Em vez de edições genéricas no registro que comprometem a estabilidade do sistema, o RiukyoX opera na camada de kernel do Windows, no agendamento de threads e no gerenciamento de memória em tempo real.

Desenvolvido para eSports e jogos competitivos, onde a precisão de entrada e a estabilidade de frametime se medem em milissegundos.

---

## RiukyoX vs. Otimizadores Genéricos

| Critério | RiukyoX | Otimizadores Comuns | Scripts Batch (.bat) |
|---|---|---|---|
| **Estabilidade de Frametime (1% Low FPS)** | **Alta consistência** via agendamento dinâmico | Melhora moderada, com picos | Instável, sem monitoramento |
| **Resposta de Clique do Mouse** | **Timer Resolution em Kernel (<0.5ms)** | Ajuste estático simples | Não trata a camada de input |
| **Consumo de Memória (RAM)** | **~40MB** (Runtime Rust nativo) | 150MB - 300MB (Electron) | 0MB (sem execução ativa) |
| **Segurança do Registro** | **Failsafe automático e restauração rápida** | Backup manual raro | Edição direta sem reversão |
| **Atualizações Automáticas** | **Motor de otimização atualizado via Nuvem** | Atualizações esporádicas | Nenhuma manutenção |

---

## Recursos Principais

<table>
<tr>
<td width="50%">

### Kernel Timer Resolution
Trava dinâmica de resolução de timer em até **0.5ms**, reduzindo a variação de clock (*jitter*) e garantindo respostas de clique consistentes.

</td>
<td width="50%">

### Win32 Process Scheduling
Alocação inteligente de *CPU Quantum* para o processo do jogo em primeiro plano, priorizando os núcleos físicos de maior frequência.

</td>
</tr>
<tr>
<td width="50%">

### Zero-Bloatware Cleaner
Desativação segura de rotinas de telemetria e serviços secundários, liberando ciclos de CPU e I/O de disco para o jogo.

</td>
<td width="50%">

### Network Bufferbloat Control
Ajuste fino da pilha TCP/IP e pacotes de rede para minimizar variações de ping e prevenir o travamento por *bufferbloat*.

</td>
</tr>
<tr>
<td colspan="2" align="center">

### Crystal Razor Glass UI
Interface desenvolvida em **Svelte 5 + WebView2** com aceleração por hardware VRAM — fluidez visual sem competir por recursos com o seu jogo.

</td>
</tr>
</table>

---

## Requisitos do Sistema & Compatibilidade

| Componente | Mínimo | Recomendado |
|---|---|---|
| **Sistema Operacional** | Windows 10 (64-bit) | Windows 11 23H2+ (64-bit) |
| **Processador** | Qualquer CPU x64 (1.0GHz+) | Quad-Core 2.5GHz+ x64 |
| **Memória RAM** | 2 GB | 4 GB ou superior |
| **Espaço em Disco** | 60 MB | 100 MB |
| **Playbook & Sistemas** | Windows Oficial / Custom ISOs | **RiukyOS Playbook (100% Integrado)** |

---

## Instalação Rápida

1. **Baixar o Instalador:** Faça o download do arquivo executável [riukyox-wizard.exe](https://github.com/Riukyo/RiukyoX/releases/download/v1.0.7/riukyox-wizard.exe).
2. **Executar como Administrador:** Clique com o botão direito sobre o arquivo e selecione *"Executar como administrador"*.
3. **Aplicar Otimizações:** Abra o RiukyoX e selecione os ajustes desejados no Painel Principal.

---

## Perguntas Frequentes (FAQ)

<details>
<summary><strong>O RiukyoX pode causar banimento em Anti-Cheats (Vanguard, EAC, BattEye)?</strong></summary>
<br/>

Não. O RiukyoX opera estritamente nas configurações do **Sistema Operacional** utilizando APIs públicas do Windows. Ele não realiza injeção de código em processos de jogos, não lê a memória do jogo e não altera arquivos de títulos ou de anti-cheats.

</details>

<details>
<summary><strong>Como funcionam as atualizações automáticas?</strong></summary>
<br/>

O aplicativo possui um verificador nativo que consulta o canal oficial de releases. Quando uma nova versão fica disponível, você recebe uma notificação direta no painel e a atualização é aplicada de forma limpa e transparente.

</details>

<details>
<summary><strong>O RiukyoX é compatível com o RiukyOS Playbook e ISOs customizadas?</strong></summary>
<br/>

Sim! O RiukyoX é **100% otimizado e recomendado para uso com o RiukyOS Playbook**, além de funcionar em instalações oficiais do Windows 10/11 e ISOs modificadas (ReviOS, AtlasOS, etc.).

</details>

<details>
<summary><strong>O aplicativo é compatível com notebooks e laptops?</strong></summary>
<br/>

Sim. O RiukyoX reconhece o status de alimentação do dispositivo e adapta os perfis para evitar consumo excessivo de bateria quando desconectado da tomada.

</details>

---

<div align="center">

### Suportado em Todos os Processadores & Placas de Vídeo

<br />

<img src="https://raw.githubusercontent.com/Riukyo/RiukyoX/main/assets/intel.svg" height="28" alt="Intel" /> &nbsp;&nbsp;&nbsp;&nbsp;
<img src="https://raw.githubusercontent.com/Riukyo/RiukyoX/main/assets/amd.svg" height="28" alt="AMD" /> &nbsp;&nbsp;&nbsp;&nbsp;
<img src="https://raw.githubusercontent.com/Riukyo/RiukyoX/main/assets/nvidia.svg" height="28" alt="NVIDIA" /> &nbsp;&nbsp;&nbsp;&nbsp;
<img src="https://raw.githubusercontent.com/Riukyo/RiukyoX/main/assets/microsoft-windows.svg" height="28" alt="Windows" />

<br /><br />

### Comunidade & Suporte

Acompanhe novidades, envie feedbacks e participe do canal oficial:

**[Entrar no Servidor do Discord](#)**

<br />

© 2026 **RiukyoX**. All rights reserved.

</div>
