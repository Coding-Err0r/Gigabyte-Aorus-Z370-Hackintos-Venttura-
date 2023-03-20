<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->

<a name="readme-top"></a>

<br />
<div align="center">
  <a href="https://rhine-one.vercel.app">
    <img src="images/logo.png" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">Gigabyte Aorus Z370 Gaming 3 + i5 8600k + Ventura</h3>

  <p align="center">
    <a href="https://osxinfo.net/konu/basarili-kurulum-intel-i5-8600k-msi-b365m-pro-vh-macos-monterey.24933/">Thanks To</a>
    <br />
    <br />
  </p>
</div>

<!-- TABLE OF CONTENTS -->

<!-- ABOUT THE PROJECT -->

## About The Project

Made with Olarila EFI . This built uses the built-in IGPU.
My specs:

Processor : i5 8600k

Gpu : UHD 630

Ram: 8gb 2400Mhz

Mobo: Gigabyte Aorus Z370 Gaming 3

PSU: Gorsair 750 Watt

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- GETTING STARTED -->

## Demo Images

<img src="images/1 (1).png" alt="Logo" width="800" height="400">
<img src="images/1 (2).png" alt="Logo" width="800" height="400">
<img src="images/1 (3).png" alt="Logo" width="800" height="400">

## DeviceProperties

- IGPU patch for UHD 630
  ```sh
  <dict>
            <key>PciRoot(0x0)/Pci(0x1F,0x3)</key>
            <dict>
                <key>AAPL,slot-name</key>
                <string>Internal@0,31,3</string>
                <key>device-id</key>
                <data>cKEAAA==</data>
                <key>device_type</key>
                <string>Audio device</string>
                <key>model</key>
                <string>200 Series PCH HD Audio</string>
            </dict>
            <key>PciRoot(0x0)/Pci(0x2,0x0)</key>
            <dict>
                <key>AAPL,ig-platform-id</key>
                <data>AACSPg==</data>
                <key>AAPL,slot-name</key>
                <string>Internal@0,2,0</string>
                <key>device-id</key>
                <data>kj4AAA==</data>
                <key>device_type</key>
                <string>VGA compatible controller</string>
                <key>enable-hdmi20</key>
                <data>AQAAAA==</data>
                <key>framebuffer-con1-enable</key>
                <data>AQAAAA==</data>
                <key>framebuffer-con1-type</key>
                <data>AAgAAA==</data>
                <key>framebuffer-con2-enable</key>
                <data>AQAAAA==</data>
                <key>framebuffer-con2-type</key>
                <data>AAgAAA==</data>
                <key>framebuffer-fbmem</key>
                <data>AACQAA==</data>
                <key>framebuffer-patch-enable</key>
                <data>AQAAAA==</data>
                <key>framebuffer-stolenmem</key>
                <data>AAAwAQ==</data>
                <key>framebuffer-unifiedmem</key>
                <data>AAAAgA==</data>
                <key>hda-gfx</key>
                <string>onboard-1</string>
                <key>model</key>
                <string>Intel UHD Graphics 630</string>
                <key>enable-dpcd-max-link-rate-fix</key>
                <data>AQAAAA==</data>
                <key>dpcd-max-link-rate</key>
                <data>FAAAAA==</data>
            </dict>
        </dict>
  ```

### Boot Arguments

- Important
  ```sh
  <dict>
  			<key>boot-args</key>
  			<string>-v alcid=1 watchdog=0 -wegnoegpu dk.e1000=0 e1000=0</string>
  			<key>csr-active-config</key>
  			<data>/w8AAA==</data>
  			<key>prev-lang:kbd</key>
  			<data></data>
  			<key>run-efi-updater</key>
  			<string>No</string>
  		</dict>
  ```
