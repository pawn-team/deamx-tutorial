# deamx-tutorial
0️⃣0️⃣0️⃣1️⃣: Como utilizar DeAMX em terminal linux (Android/PC)

**OBS:** O mesmo processo vale para computador linux!

**Passo 1:** Atualizar os pacotes do Termux
- **Descrição:** Este passo garante que os pacotes do Termux estejam atualizados, o que é importante para obter as versões mais recentes dos programas.
- **Comandos:** `yes | pkg update -y && yes | pkg upgrade -y`

**Passo 2:** Obter permissão para acessar memória externa
- **Descrição:** Este passo permite que o Termux acesse a memória externa do seu dispositivo, onde você pode armazenar ou recuperar arquivos.
- **Comandos:** `termux-setup-storage`

**Passo 3:** Instalar os pacotes Git e Lua v5.1
- **Descrição:** Esses pacotes são necessários para o processo de clonagem e decompilação.
- **Comandos:** `pkg install git lua51 -y`

**Passo 4:** Clonar o repositório do decompilador DeAMX
- **Descrição:** Isso baixa o código-fonte do decompilador DeAMX para o seu dispositivo.
- **Comandos:** `git clone https://github.com/AmyrAhmady/DeAMX $HOME/DeAMX`

**Passo 5:** Abrir o diretório clonado
- **Descrição:** Navegue até a pasta onde você clonou o repositório DeAMX.
- **Comandos:** `cd $HOME/DeAMX`

**Passo 6:** Copiar o binário do gamemode que deseja decompilar
- **Descrição:** Este passo envolve copiar o arquivo do gamemode que você deseja decompilar para a pasta do decompilador.
- **Comandos:** `cp -r /sdcard/Download/sampserver/gamemodes/base.amx $PWD`

**Passo 7:** Usar o comando para decompilar
- **Descrição:** Este comando executa o processo de decompilação do gamemode usando o Lua.
- **Comandos:** `lua51 deamx.lua base.amx`

**Passo 8:** Mover o arquivo PWN para a pasta do gamemode
- **Descrição:** Após a decompilação, o arquivo PWN gerado é movido de volta para a pasta do gamemode.
- **Comandos:** `mv base.pwn /sdcard/Download/sampserver/gamemodes`

Siga o canal para receber notificações de novos métodos, projetos, dicas e tutoriais!
Com carinho, DeviceWhite 😀👍
