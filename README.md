# Optimus-mainboard-firmware
Firmware with original delta calibration for Optimus mainboard (before the slider orientation changed).

I think the bigger calibration pattern is not needed, so I branched the last version with the original calibration pattern.
I will add my modifications to both branches, the master branch and this "original-calibration" branch.

## TTL laser control
This branch additionally contains configuration adjustments to use the TTL connection like I described here:
https://www.febtop.com/forum/technical-issues/solved-using-ttl-for-the-laser-module

Instead of controlling the laser power with PIN 2.4 (24V) using PWM this solution uses PIN 1.23 (3V) to connect to the TTL PIN of the laser board using PWM. The laser power is provided by PIN 2.7 (24V) that is configured to be always on.
