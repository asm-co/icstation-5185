# icstation-5185
ICStation 8 Channel MICRO USB Relay Module 5V ICSE014A

http://www.icstation.com/icstation-channel-micro-relay-module-icse014a-p-5185.html

![ICStation 5185](http://www.icstation.com/images/big/productimages/5185/5185.jpg)

## Usage

* Install windows GUI or implement the following serial protocol directly.
* USB-to-Serial IC is Prolific PL-2303HX [OSX Driver Download](http://www.prolific.com.tw/US/ShowProduct.aspx?p_id=229&pcid=41)

### Protocols

```0x50 0x51 0xQQ```

* 0x50 -- Activate module (send once per session to enable receipt of commands)
* 0x51 -- Command signature (indicates subsequent byte is relay state)
* 0xQQ -- Bit packed relay state information (0 = closed/on; 1 = open/off)

### Notes

* Power the relay from the header pin instead of the power jack. There appears to be a big voltage drop on the power jack.
* https://www.youtube.com/watch?v=yasznSglN2s
