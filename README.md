# Arduino - AVR GCC multiplication

This is a fork of Norbert Pozar's AVR GCC multiplcation macros.  My
modifications:
- Added support for fractional 1.15 numbers.  I haven't added support
  for everything possible, just the stuff I need.
- GCC asm statements improved to avoid clobbering hardcoded registers
  and instead let GCC decide which registers to use.
- Removed "volatile" from asm statements to let GCC decide whether the
  code is necesssary or can be eliminated.

TODO:
- Make functional macros for everything instead of specifying a result
  variable as an argument.

## Original README:

Implementation of various multiplication routines for AVR microprocessor. Tested on ATmega168 (Arduino).

See [my blog article](http://mekonik.wordpress.com/2009/03/18/arduino-avr-gcc-multiplication/) for details.

You can do anything you want with the code. I release it to *public domain*.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

---

Norbert Pozar 2009
