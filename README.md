# Dell Vostro 5581

This build running on MacOs X

# System specification

    1.Name:           Dell Vostro 5581
    2.CPU:            Intel Core i7-8565U
    3.Graphic:        Intel UHD620
    4.Wifi:           REPLACED WITH DW1560 (AirDrop and Handoff Working perfectly)
    ------------------------------------------------------------------------------
    Display: OK
    Audio ALC 236/Audio HDMI: OK
    Headphone fix: https://www.elitemacx86.com/threads/fix-audio-distortion-when-using-headphones-on-laptops.185/
    Battery: OK
    Type-C: OK
    HDMI: OK
    FN Hotkey: OK
    Trackpad: OK
    Sleep: OK
    IMES/Facetime: OK

# Step to install(Clover)

    1. Run and Install Clover_v2.5k_r5058.pkg with EFI 
    2. Replace Clover folder in EFI partition
    3. Trackpad: Move CodecCommander.kext in Trackpad/LE and KextBeast to Desktop, run KextBeast select L/E
    4. Enjoy
    5(Optional): Enable HiDPi https://github.com/xzhih/one-key-hidpi

# Step to install(Opencore)

    1. Mount EFI folder 
    2. Copy OC vs Boot to EFI
    3. Gen SMBIOS https://github.com/corpnewt/GenSMBIOS
    4. Enjoy