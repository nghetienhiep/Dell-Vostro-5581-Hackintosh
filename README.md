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