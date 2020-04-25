# es_extended
FUSED WITH ESSENTIALMODE

es_extended is a roleplay framework for FiveM. ESX is short for EssentialMode Extended. The to-go framework for creating an economy based roleplay server on FiveM and most popular on the platform, too!

Featuring many extra resources to fit roleplaying servers, here's a taste of what's available:

esx_ambulancejob: play as a medic to revive players who are bleeding out. Complete with garages and respawn & bleedout system
esx_policejob: patrol the city and arrest players commiting crime, with armory, outfit room and garages
esx_vehicleshop: roleplay working in an vehicle dealership where you sell cars to players
ESX was initially developed by Gizz back in 2017 for his friend as the were creating an FiveM server and there wasn't any economy roleplaying frameworks available. The original code was written within a week or two and later open sourced, it has ever since been improved and parts been rewritten to further improve on it.

Links & Read more

- ESX Documentation
- ESX Development Discord
- FiveM Native Reference

Features

Weight based inventory system
Weapons support, including support for attachments and tints
Supports different money accounts (defaulted with cash, bank and black money)
Many official resources available in our GitHub
Job system, with grades and clothes support
Supports multiple languages, most strings are localized
Easy to use API for developers to easily integrate ESX to their projects
Register your own commands easily, with argument validation, chat suggestion and using FXServer ACL

Requirements

mysql-async
async

Manually

Download https://github.com/ESX-Org/es_extended/releases/latest
Put it in the resource/[essential] directory
Download https://github.com/ESX-Org/esx_menu_default/releases/latest
Put it in the resource/[esx]/[ui] directory
Download https://github.com/ESX-Org/esx_menu_dialog/releases/latest
Put it in the resource/[esx]/[ui] directory
Download https://github.com/ESX-Org/esx_menu_list/releases/latest
Put it in the resource/[esx]/[ui] directory

Installation

Import es_extended.sql in your database
Configure your server.cfg to look like this

add_principal group.admin group.user
add_ace resource.es_extended command.add_ace allow
add_ace resource.es_extended command.add_principal allow
add_ace resource.es_extended command.remove_principal allow
add_ace resource.es_extended command.stop allow

start mysql-async
start es_extended

start esx_menu_default
start esx_menu_list
start esx_menu_dialog
