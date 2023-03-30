# <span style="color: red;">Dự án đã dừng lại năm 2023. Tôi đã không sử dụng thiết bị này nữa.</span>

# Dell Vostro 5581

This build running on MacOs X

# System specification
<ol>
  <li>Name: Dell Vostro 5581</li>
  <li>CPU: Intel Core i7-8565U</li>
  <li>Graphic: Intel UHD620</li>
  <li>Wifi: REPLACED WITH DW1560 (AirDrop and Handoff Working perfectly)</li>
</ol>

------------------------------------------------------------------------------
<ul>
  <li>Display: OK</li>
  <li>Audio ALC 236/Audio HDMI: OK</li>
  <li>Battery: OK</li>
  <li>Type-C: OK</li>
  <li>HDMI: OK</li>
  <li>FN Hotkey: OK</li>
  <li>Trackpad: OK</li>
  <li>Sleep: OK</li>
  <li>IMES/Facetime: OK</li>
</ul>

# Step to install(Clover)

<ol>
  <li>Run and Install Clover_v2.5k_r5058.pkg with EFI </li>
  <li>Replace Clover folder in EFI partition</li>
  <li>Trackpad: Move CodecCommander.kext in Trackpad/LE and KextBeast to Desktop, run KextBeast select L/E</li>
  <li>Enjoy</li>
  <li>(Optional) Enable HiDPi <a href="https://github.com/xzhih/one-key-hidpi" target="_blank">Link</a></li>
</ol>

# Step to install(Opencore)

<ol>
  <li>Mount EFI folder </li>
  <li>Copy OC vs Boot to EFI</li>
  <li>Gen SMBIOS <a href="https://github.com/corpnewt/GenSMBIOS" target="_blank">Link</a></li>
  <li>Enjoy</li>
</ol>

# Wifi Intel (No airdrop, handoff)

Source: https://github.com/OpenIntelWireless

<ol>
  <li>Remove kexts: <strong>AirportBrcmFixup.kext, BlueToolFixup.kext, BrcmFirmwareData.kext, BrcmPatchRAM3.kext, BrcmBluetoothInjector.kext</strong> in <strong>OC/Kexts</strong></li>
  <li>Choose 1 of 2 kext: <strong>itlwm.kext</strong> or <strong>itlwmx.kext</strong> and copy to <strong>OC/Kexts</strong> (Notes below)</li>
  <li>Update the config file with ProperTree</li>
  <li>Download and copy the HeliPort app to the Applications folder</li>
  <li>Reboot</li>
  <li>Run Heliport select wifi and connect</li>
</ol>

## itlwm.kext

|PCI ID|Device_Name|
|---|---|
|0x08b1|AC 7260|
|0x08b2|AC 7260|
|0x08b3|AC 3160|
|0x08b4|AC 3160|
|0x095a|AC 7265|
|0x095b|AC 7265|
|0x3165|AC 3165|
|0x3166|AC 3165|
|0x24f3|AC 8260|
|0x24f4|AC 8260|
|0x24f5|AC 4165|
|0x24f6|AC 4165|
|0x24fb|AC 3168|
|0x24fd|AC 8265|
|0x2526|AC 9260|
|0x9df0|AC 9560|
|0xa370|AC 9560|
|0x31DC|AC 9560|
|0x30DC|AC 9560|
|0x271C|AC 9560|
|0x271B|AC 9560|
|0x42a4|AC 9462|
|0x00a0|AC 9462|
|0x00a4|AC 9462|
|0x02a0|AC 9462|
|0x02a4|AC 9462|
|0x40a4|AC 9462|
|0x0060|AC 9461|
|0x0064|AC 9461|
|0x0260|AC 9461|
|0x0264|AC 9461|

## itlwmx.kext

|PCI ID|Device_Name|
|---|---|
|0x2723|AX200|
|0x2720|AX201|
|0x43F0|AX201|
|0xA0F0|AX201|
|0x34F0|AX201|
|0x02F0|AC 9462|
|0x3DF0|AC 9462|
|0x06F0|AX201|
