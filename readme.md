## AirGradientUpgrades

**Note: this software is aimed to only the AirGradient Pro 3.7 with TVOC.** You can certainly adapt this script if you don't have the TVOC module in your Air Gradient.

This modification adds a http /metrics (for prometheus), and a /metricsjson endpoint on port 8080.

This script is not written from the ground up by any means. The base of this script was taken from https://github.com/airgradienthq/arduino. To make it easy to tell what was modified, all bits of code added by me have a comment denoting that.

### Setup

Clone this repo and open `air_gradient/air_gradient.ino`. Install all libraries at the correct version listed in the comment. After installing those libraries, additionally install `AirGradient Air Quality Sensor`.

Then, downgrade EspSoftwareSerial to version `6.17.1`. As of right now, version 7.0.0 causes frequent crashes. (Thank you to ken830 on the Air Gradient fourms for putting in a lot of work to figure this out!)