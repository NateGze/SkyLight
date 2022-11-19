# SkyLight

You need to add both the SkyLight and Skylight Room code to your Hubitat Apps Code.

Install Skylight, restart app and then add new automations on a room by room basis.

Will support operation without a master switch with devices that provide some sort of feedback when either they are turned off, or some sort of reachback information when they are turned on (may be light level or color temperature, or both). Reachback values to search for can be either of those number sources, it will search for both of them to check for a match.

It is known that certain Sengled LEDs will send a signal saying they have been turned off when you kill power to them.  Philips hue will send a reachback value when turned on and refreshed while being paired through their hub. It is known that this app will work without a master switch with Sengleds, and philips hue (with a frequent refresh value). Their may be others.
