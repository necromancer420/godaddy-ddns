# godaddy-ddns
Simple Dynamic DNS Service for Godaddy Servers
|:--:| 
| Assumes '@' for A-Name on Godaddy DNS |

## Purpose
Update The A Record of your domain on Godaddy DNS to your current IP Address. 
(Useful for ISPs that constantly change your home IP address)

## Usage
Be sure to get your API Key from Godaddy before using the script.

You must change the domain name & API Key fields in the dyndnsgd script

The Script Can be run manually, but would be best used as a cron job.

## Installation
```bash
cd ~/Downloads
git clone https://github.com/necromancer420/godaddy-ddns.git
cd godaddy-ddns
chmod +x dyndnsgd
./dyndnsgd
```
or add the script to your crontab...
```bash
sudo crontab -e
```
Add the following line to the bottom of the file 
```bash
*/10 * * * *    ~/Downloads/godaddy-ddns/dyndnsgd > /dev/null
```
Save the file and exit, then Reboot.

## License
[Unilicense](https://choosealicense.com/licenses/unlicense/#)
This is free and unencumbered software released into the public domain.

Anyone is free to copy, modify, publish, use, compile, sell, or
distribute this software, either in source code form or as a compiled
binary, for any purpose, commercial or non-commercial, and by any
means.

In jurisdictions that recognize copyright laws, the author or authors
of this software dedicate any and all copyright interest in the
software to the public domain. We make this dedication for the benefit
of the public at large and to the detriment of our heirs and
successors. We intend this dedication to be an overt act of
relinquishment in perpetuity of all present and future rights to this
software under copyright law.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
OTHER DEALINGS IN THE SOFTWARE.

For more information, please refer to <https://unlicense.org>

---------
