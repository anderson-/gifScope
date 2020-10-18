# gifScope
> Python script to generate GIFs from a USB oscilloscope 

Should work on some GW Instek scopes, tested on a MO-2062/GDS-1000A (Minipa)

![](/img1.png)

![](/img2.gif)

# Requisites

- Python 3.6+
- pySerial
- PIL

# Usage

- Check scope response: `./gifScope /dev/ttyACM0 -t`
- Take a png screenshot: `./gifScope /dev/ttyACM0 out.png`
- Take a jpg screenshot: `./gifScope /dev/ttyACM0 out.jpg`
- Record a 10 seconds GIF: `./gifScope /dev/ttyACM0 -g 10 out.gif`
- Record a gif, no timeout: `./gifScope /dev/ttyACM0 -g out.gif`

# Licence

Distributed under the GNU General Public License. See LICENSE for more information.

# Acknowledgements

Thanks to [@yytseng and Thomas Weidenfeller](https://github.com/yytseng/gds2000tools) who made this possible.