# pfsense2.6-pfblocker-log
pfsense 2.6 - pfblocker sem gerar log

Após atualização do PfSense para versão 2.6 os logs do PfBlocker parou de funcionar, executei os comandos abaixo para voltar a funcionar.

Entre no menu "Diagnóstico/Prompt de Comando"
Coloque o comando abaixo

> cp /usr/local/pkg/pfblockerng/pfblockerng.inc{,.bkp}

########################################################

Clique em Executar

Coloque o comando abaixo
> curl -o /usr/local/pkg/pfblockerng/pfblockerng.inc "https://gist.githubusercontent.com/BBcan177/7cb8635199446866d511b97166d65296/raw/"

OU este comando abaixo que é uma cópia do arquivo do repositório acima.

> curl -o /usr/local/pkg/pfblockerng/pfblockerng.inc "https://raw.githubusercontent.com/admredesmaiconalves/pfsense2.6-pfblocker-log/main/pfblockerng.inc"


Clique em Executar

########################################################

Entre no menu "Status/Serviços"
Reinicie o serviço pfb_filter

Verifique os logs do PfBlocker.
