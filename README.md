# edgeIPass - fork of the PassIFox and chromeIPass project from pfn's github.

These are extensions to integrate [KeePass](http://keepass.info)/[KeePassXC](https://keepassxc.org/) as a password manager with the different browsers.  As a basic test using Microsoft's Edge Extension Toolkit for conversion, I've replaced the chromeipass folder with an edgeipass folder, and made the various changes to get the tool working with Edge

It also requires [KeePassHttp](https://github.com/pfn/keepasshttp/), a KeePass plugin to expose password entries securely (256bit AES/CBC) over HTTP.

For edgeIPass to work properly, you will need to run the following in Windows PowerShell as an admin:
CheckNetIsolation LoopbackExempt -a -n="Microsoft.MicrosoftEdge_8wekyb3d8bbwe"

This allows for the extension to make connections to KeePassHTTP on the loopback address.

A few additional notes:
It looks like edge doesn't support the listener for the CTRL+U and CTRL+P keyboard shortcuts (although I didn't look too hard to figure that out).

I'm currently running this from the latest Windows Insider build of the upcoming Fall update (build 16291). I'm assuming it will work on the current version, but just in case it doesn't that may be why.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.
