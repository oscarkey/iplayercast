# iPlayercast
Copyright 2013 Oscar Key  
Licensed under GPL v3. See below and LICENSE.  
A python script that downloads BBC iPlayer programmes and builds them into a podcast feed.  

The script searches iPlayer for the given programmes and downloads them. It then produces a podcast xml feed which could be subscribed to with a podcast reader application. In order for this to happen the output directory should be served by a webserver. It uses get-iplayer to retrieve the programmes, thus it and all its dependancies must be installed.

**Usage:** python3 iplayercast -c [config directory]  
[config directory] should contain:  

- iplayercast.conf (the main config file)  
- feeds (directory containing feed.conf files)  

I recommend running it using a bash script which is then called by cron every few hours. The output directory should be served by a webserver. See the sample config files for configuration examples.

**Do not use the script to produce public podcasts, it is for personal use only. If you publically serve programmes you may be in violation of the BBC's copyright.**

## LICENSE
This program is free software: you can redistribute it and/or modify  
it under the terms of the GNU General Public License as published by  
the Free Software Foundation, either version 3 of the License, or  
(at your option) any later version.

This program is distributed in the hope that it will be useful,  
but WITHOUT ANY WARRANTY; without even the implied warranty of  
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the  
GNU General Public License for more details.

You should have received a copy of the GNU General Public License  
along with this program.  If not, see <http://www.gnu.org/licenses/>.
