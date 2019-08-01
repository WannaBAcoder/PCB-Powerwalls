# PCB-Powerwalls
This is the public file Repository for the DIY PCB Powerwall Community

We are developing a PCB alternative to common powerwall building techniques for 18650(and similar) batteries. This system has been developed with maintainability, expandability, and practicality in mind.

## 15s4p PCB

The 15s4p battery board is a stackable solution that reduces the amount of wiring required by placing all series and balance connections through standoffs that structurally connect the boards. Batteries mount to both sides of the PCB, in a variety of ways. Each cell is individually fused for added safety.

**1. Plastic battery holders**

You can choose to use plastic cell holders that are available in many through-hole, and surface mount packages. For the through-hole packages, you must bend the pins at a 90 degree angle so that the holders sit as flat as possible.

![Top view](https://github.com/WannaBAcoder/PCB-Powerwalls/blob/master/15s4p_PCB/Renders/holder_top.jpg)
![Iso view](https://github.com/WannaBAcoder/PCB-Powerwalls/blob/master/15s4p_PCB/Renders/holder_side.jpg)

**2. Spring Clips**

A cheaper alternative to plastic holders is spring clips. The clips work like traditional battery holders with springs, but these require the use of zip ties to hold the cells in place.

![Top view](https://github.com/WannaBAcoder/PCB-Powerwalls/blob/master/15s4p_PCB/Renders/15s4p_board_top.jpg)
![Iso view](https://github.com/WannaBAcoder/PCB-Powerwalls/blob/master/15s4p_PCB/Renders/15s4p_board_side.jpg)

**3. Fuse wire**

The last option is to use fuse wire. You will still need to use zip ties to hold the cells in place, but you can solder the fuse wire directly to the PCB pads, and remove the need for populating fuses(you will need to short the fuse pads to do this).

![Top view](https://github.com/WannaBAcoder/PCB-Powerwalls/blob/master/15s4p_PCB/Renders/fw_top.jpg)
![Iso view](https://github.com/WannaBAcoder/PCB-Powerwalls/blob/master/15s4p_PCB/Renders/fw_side.jpg)

### 7s Adapter PCB

The 7s Adapter PCB was created to take our popular 15s4p design and convert it into a 7s8p PCB. We do this by leaving the out the 8s cells, and connecting the other 7 strings in parallel with the first. It is recommended to use at least one of these adapter PCBs for every 5 boards, or 20A of main fuse(which is 10A load on each of these boards). This board also joins the battery stacks with standoffs. It's important to equally space these boards within a pack for best current distribution. For example, a 12 battery board stack could use 3 adapter boards, spaced every 4 boards.

![Top view](https://github.com/WannaBAcoder/PCB-Powerwalls/blob/master/7sAdapter_PCB/Renders/top.png)
![Iso view]()

### BMS/Display Adapter PCB

The BMS/display adapter board helps the user connect a [Moonitor](link to Moonitor), or a variety of BMS systems to the battery PCB stacks, and is capable of supporting ~5A balance current. This board also includes spaces to add string-level voltage displays, but they can be disabled if not desired.  You can also use this board with the 7s adapter board configurations. Visit the wiki to find out how. (insert wiki link here once it exists)

![Top view](https://github.com/WannaBAcoder/PCB-Powerwalls/blob/master/BMS_display_adapter_PCB/Renderings/top.png)
![Iso view](https://github.com/WannaBAcoder/PCB-Powerwalls/blob/master/BMS_display_adapter_PCB/Renderings/side.png)

## Building Your Own

You can order your own board at any number of PCB manufacturers. Many of our supporters use [JLCPCB.com](https://jlcpcb.com/quote).

### The standard order
*PCB thickness-1.6mm
*PCB Color-Your choice (black is not available for 2oz copper orders)
*Surface finish - HASL(with lead)
*Copper Weight - 1oz or 2oz. Higher current applications use 2oz.
*All other opeions can be left as default.


link to wiki?



## Versioning

Each powerwall PCB has its own revision in the form of VX.X. In addition to this, we version the entire system package in a release in the form of RX.0. See the latest release for the most recent hardware package. Whenever any of the hardware in a package changes, the PCB version and package release will be updated. PCB versions are printed on all PCBs for easy identification.

## Contributing

Although the kicad source files are available, the safety considerations that go into this project make it potentially unsafe to modify. Do so at your own risk. You can always contribute tothe development of this project by suggesting hardware updates by reporting an [issue](https://github.com/WannaBAcoder/PCB-Powerwalls/issues).

## License

This project is licensed under the CERN Open Hardware License - see the [LICENSE.txt](LICENSE.txt) file for details.

## Acknowledgments

A special thank you to the people that helped develop the early versions of this hardware and helped others realize the growing potential for these designs:
* Shaun Bond
* Izz Eselam
* Paulo E Cabigao
* Dale Bliss
