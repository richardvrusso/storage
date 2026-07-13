<style>
  table {
    border-collapse: collapse !important;
    width: 100%;
    margin-bottom: 20px;
  }
  th, td {
    border: 1px solid #224422 !important; /* Faint matrix-green lines to match the Hacker theme */
    padding: 10px !important;
  }
  /* Force all images in the first column to be exact 60x60 pixel squares */
  td:first-child img {
    width: 300px !important;
    height: 300px !important;
    object-fit: contain !important; /* Prevents the image from stretching or distorting */
    background-color: transparent;  /* Keeps it clean on the dark background */
</style>
[← Back to Main Homelab Hub](https://richardvrusso.github.io/homelab/)

# unRAID Storage Server
Running unRAID serving as a storage server for the homelab. In an emergency, it can host Docker and VMs.

| Preview | Product Name | Component Specifications & Notes |
| :---: | :--- | :--- |
| ![Chassis](https://m.media-amazon.com/images/I/51gSRzTWhfL._AC_SL1500_.jpg) | [Rosewill 4U Server Chassis 9 Bay Server Case](https://a.co/d/08OKxhuC){:target="_blank"} | Standard 4U rackmount enclosure<br>• *Provides 9 internal/external expansion bays for high-density storage layout* |
| ![Motherboard](https://m.media-amazon.com/images/I/81833wyfcEL._AC_SL1500_.jpg) | [ASRock Rack Motherboard E3C236D4U](https://a.co/d/0bhX6TCu){:target="_blank"} | Enterprise Micro-ATX server board (Intel C236 chipset)<br>• *Features dual Gigabit LAN ports and native IPMI management* |
| ![CPU](https://m.media-amazon.com/images/I/61W4angoAHL._AC_SL1200_.jpg) | [Intel Xeon E3-1270 v6 Quad-core Processor](https://a.co/d/0dEbSwoh){:target="_blank"} | 4 Cores / 8 Threads, 3.80 GHz base clock (Kaby Lake)<br>• *Reliable computing power with integrated Intel HD Graphics P630* |
| ![RAM](https://c1.neweggimages.com/productimage/nb1280/C0XKD2603010YSAWF57.jpg) | [Samsung 16GB 2X8GB PC4-2133P DDR4 ECC UDIMM](https://www.newegg.com/p/3C6-0008-00993){:target="_blank"} | 2133MHz unbuffered enterprise server memory<br>• *ECC error-correcting capabilities ensures high system uptime and data integrity* |
| ![NVMe](https://m.media-amazon.com/images/I/41IAIyvic4L._AC_.jpg) | [Toshiba XG6 KXG60ZNV512G 512GB NVMe M.2 SSD](https://a.co/d/04Do2F2E){:target="_blank"} | High-speed M.2 2280 form-factor solid state drive<br>• *Serves as an ideal lightning-fast application host or cache drive* |
| ![SATA SSD](https://m.media-amazon.com/images/I/81HNEuqdlfL._AC_SL1500_.jpg) | [Samsung SSD 860 EVO 4TB 2.5 Inch SATA III SSD](https://a.co/d/00WG5w5x){:target="_blank"} | High-capacity 2.5" high-endurance flash storage<br>• *Massive 4TB solid-state block for heavy read/write container or VM workloads* |
| ![PSU](https://c1.neweggimages.com/productimage/nb1280/17-139-333-04.png) | [CORSAIR RM550x 550 Watt 80+ Gold Fully Modular PSU](https://www.newegg.com/corsair-rmx-series-atx-3-1-compatible-850-w-cybenetics-gold-power-supply-black-rm850x/p/N82E16817139333?Item=N82E16817139333){:target="_blank"} | Premium efficiency compact ATX power supply unit<br>• *Fully modular cables ensure clean airflow optimization throughout the 4U chassis* |
| ![Fan](https://m.media-amazon.com/images/I/91JkAMy5xQL._SL1500_.jpg) | [Noctua NF-P12 redux-1300 PWM 120mm 4-Pin Fan](https://a.co/d/0cta5wOM){:target="_blank"} | High-pressure pressure-optimized quiet cooling unit<br>• *Note: System utilizes custom configurations/wrappers to support legacy 3-pin chassis requirements* |
| ![NIC](https://i.ebayimg.com/images/g/t0sAAeSw1adpp~TQ/s-l1600.webp) | [Mellanox MNPA19-XTR 10G Connectx-2 PCIe SFP+ NIC](https://www.ebay.com/itm/196321104392){:target="_blank"} | Enterprise PCI Express 10 Gigabit SFP+ fiber network adapter<br>• *Establishes ultra-fast 10GbE network fabric backend uplink to main switch* |
| ![Cable](https://m.media-amazon.com/images/I/51SK0aIAJhL._SL1008_.jpg) | [H!Fiber.com 2 Pack 10G SFP+ DAC Cable 2M](https://a.co){:target="_blank"} | Twinax passive network patch link assemblies<br>• *One for unRAID server and one for storage server* |
| ![Thermal Compound](https://m.media-amazon.com/images/I/71IyZUF9EPL._AC_SL1500_.jpg) | [Thermal Grizzly Conductonaut Thermal Grease](https://a.co/d/00xBkMIQ){:target="_blank"} | Liquid metal high-performance thermal interface compound<br>• *Maximizes heat dissipation between Xeon IHS and cooling arrays* |
