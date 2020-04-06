# <img src="https://raw.githubusercontent.com/dpteam/AwesomeDPT-WindowsSoft/master/content/logo.png?raw=true" width="400">

💻 Скрипт интеграции Windows Store для Windows 10 Enterprise 2015 / 2016 LTSB или Windows Enterprise 2015 / 2016 LTSB N / 2019 LTSC / Server 2016

## Ссылки

- [AwesomeDPT](https://dpteam.github.io/AwesomeDPT) - Вернуться в основной список.

## Чтобы установить, запустите Add-Store.cmd от имени администратора. 
Если вы не хотите, чтобы установились App Installer / Purchase App / Xbox identity, удалите каждый пакет appxbundle перед запуском установки. Однако, если вы планируете установить игры или какое-либо приложение с опциями покупки, вы должны включить все. 

Если магазин по-прежнему не будет работать, перезагрузите компьютер. Если по-прежнему не работает, откройте командную строку от имени администратора и выполните следующую команду, а затем перезагрузите компьютер еще раз. 

```PowerShell -ExecutionPolicy Unrestricted -Command "& {$manifest = (Get-AppxPackage Microsoft.WindowsStore).InstallLocation + '\AppxManifest.xml' ; Add-AppxPackage -DisableDevelopmentMode -Register $manifest}"```    

## Устранение неполадок 
1. Правой кнопкой по пуску 
2. Выполнить 
3. Ввести: WSReset.exe 

Это очистит кеш при необходимости. 

Идея: GOD666 [https://forums.mydigitallife.net/threads/add-store-to-windows-10-enterprise-ltsc-ltsb.70741/page-22#post-1419464] 

Автор скрипта: kkkgo 

Применены фиксы от TheMooskyFIsh и Nun-z 

Русификация и оптимизация: DartPower
