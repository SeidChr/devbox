FROM mcr.microsoft.com/powershell
RUN apt-get update \
    && apt install -y git

SHELL [ "pwsh", "-Command" ]

RUN  iwr -Uri 'https://raw.githubusercontent.com/SeidChr/pwsh.files/master/setup/install.ps1' -Headers @{"Cache-Control"="no-cache"} | iex

CMD ["pwsh"]