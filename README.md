# troca_hostname
Script PowerShell para troca de hostname.

Script que realiza troca do hostname para estrutura predeterminada de máquinas Windows via PowerShell e envia feedback por e-mail.

No código de exemplo é solicitado ao usuário input de número de patrimônio e o script se encarrega de solicitar para bios o serial number do dispositivo.

Formando a seguinte estrutura: NOME-PATRIMONIO-SERIALNUMBER.

Ignora limite de tamanho de hostname.

Encaminha feedback via e-mail com novo hostname configurado e usuário que fez a alteração.

Idealizado para ser usado em conjunto com Gmail.

Necessário 2fa ativado (https://myaccount.google.com/two-step-verification/phone-numbers).

Necessário senha de app (https://myaccount.google.com/apppasswords).

Recomendado compilação com PS2EXE.

Necessário permissão administrador.

Efetivamente hostnames só são trocados no Windows após reboot do sistema, portanto, existe rotina para reboot após 30s viabilizando o envio do e-mail.


