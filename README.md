# Troubleshooting Básico & Intermediário

## Básico

### Ping
Exibir a ajuda do comando:
```sh
ping www.google.com.br
ping -t www.google.com.br
```
Referência: [Microsoft Docs - ping](https://learn.microsoft.com/pt-br/windows-server/administration/windows-commands/ping)

### Tracert
Exibir a ajuda do comando:
```sh
tracert www.google.com.br
tracert -h 5 www.google.com.br
tracert -4 -h 5 www.google.com.br
```
Referência: [Microsoft Docs - tracert](https://learn.microsoft.com/pt-br/windows-server/administration/windows-commands/tracert)

### Nslookup
Exibir a ajuda do comando:
```sh
nslookup www.google.com.br 181.213.132.2
```

### Outros comandos
- `traceroute`
- `tracepath`
- `tcping` ([Referência](https://neoctobers.readthedocs.io/en/latest/linux/tcpping_on_ubuntu.html))
- `route print`
- `dig`
- `nc` & `netcat`
- `nmap`
- `curl`
  ```sh
  curl https://bb.com.br --verbose
  ```
  [Referência](https://curl.se/docs/manpage.html)
- `mtr`
  ```sh
  sh -c 'mtr -n -z --report-cycles 10 --report 52.20.78.240'
  ```
  [Referência](https://linuxcommandlibrary.com/man/mtr)
- `LookingGlass`

## PowerShell

## WireShark

## WSL Linux
### Instalar WSL
[Guia de Instalação](https://learn.microsoft.com/pt-br/windows/wsl/install)

### Checar Interfaces
```sh
netsh interface ipv4 show subinterfaces
```
[Referência](https://learn.microsoft.com/en-us/powershell/module/netadapter/get-netadapter?view=windowsserver2022-ps)

### Manipular o MTU
```sh
netsh interface ipv4 set subinterface "vEthernet (WSL)" mtu=1490 store=persistent
```
[Referência](https://www.bemmelhor.com.br/info/index.php?title=Configurando_MTU_no_Windows)

### Testar Sites
```sh
curl https://bb.com.br --verbose
curl https://iw.claro.com.br --verbose
```

## PortScanner
- [PortForward - Network Utilities](https://portforward.com/software/download-instructions/network-utilities/)
- [Check All Open Ports Online](http://ports.my-addr.com/check-all-open-ports-online.php)
- [nPerf - Network Testing](https://www.nperf.com/pt/)

### Tools Port and Vulnerability Scanner
- [Nmap](https://nmap.org/)
- [How to Run a Vulnerability Scan Using Nmap](https://www.datamation.com/security/how-to-easily-run-a-vulnerability-scan-using-nmap/#:~:text=Nmap%20(network%20mapper)%20can%20be,experts%20perform%20scans%20for%20safety.)
- [Nmap Vulnerability Scan](https://securitytrails.com/blog/nmap-vulnerability-scan)
- [Check All Open Ports Online](http://ports.my-addr.com/check-all-open-ports-online.php)
- [PowerShell Port Scan](https://medium.com/@nallamuthu/powershell-port-scan-bf27fc754585)
- [Nmap Advanced Port Scans - TryHackMe](https://medium.com/@Aircon/nmap-advanced-port-scans-tryhackme-thm-ed3859a33eca)

## Wi-Fi Analyzer
### Windows
- Windows - Insider

### Android

---

## 📌 Como Contribuir
Se você deseja contribuir com este repositório e melhorar as informações deste README, siga estas etapas:

1. **Fork este repositório** clicando no botão "Fork" no canto superior direito da página do GitHub.
2. **Clone o repositório** para sua máquina local:
   ```sh
   git clone https://github.com/seu-usuario/seu-repositorio.git
   ```
3. **Crie uma nova branch** para suas alterações:
   ```sh
   git checkout -b minha-melhoria
   ```
4. **Edite o arquivo `README.md`** com suas melhorias, correções ou adições.
5. **Faça um commit** com uma mensagem descritiva:
   ```sh
   git add README.md
   git commit -m "Melhoria na seção de troubleshooting"
   ```
6. **Envie suas alterações para o seu repositório forkado**:
   ```sh
   git push origin minha-melhoria
   ```
7. **Crie um Pull Request (PR)** no repositório original para que suas mudanças sejam revisadas e possivelmente aceitas.

### 📌 Convensões de Commits e Pull Requests
Para manter um padrão e a organização do repositório, siga estas diretrizes:

#### Commits
- Use mensagens curtas e descritivas.
- Utilize a seguinte estrutura para mensagens de commit:
  ```sh
  tipo: breve descrição da alteração
  ```
  Exemplos:
  ```sh
  feat: adiciona nova seção de troubleshooting
  fix: corrige link quebrado em referência
  docs: melhora descrição de comando nslookup
  ```

#### Pull Requests
- Descreva claramente as mudanças feitas e o motivo.
- Adicione referências se aplicável.
- Certifique-se de que sua contribuição está formatada corretamente e testada antes de enviar.

Agradecemos sua contribuição! 🚀
