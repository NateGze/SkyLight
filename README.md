# SkyLight

You need to add both the SkyLight and Skylight Room code to your Hubitat Apps Code.

Install Skylight app, restart it, and then add new automations from there.
Automations are intended to be set up on a room by room basis.

Code will continually change color temperature throughout daylight hours to match typical color temperature values of daylight throughout the day.

Code is continually trying to make sure that bulbs that it is sending temperature changes to are still on, as to not turn bulbs back on that are being used for other things, or are intended to be off for other scenes.  Supports turning on and off a group of lights (and potentially changing levels) through a master switch. 

Will also support color temperature changing operation without a master switch with devices that provide some sort of feedback through either when they are turned off, or some sort of reachback information when they are turned on (may be light level or color temperature, or both). Reachback values to search for can be either of those number sources, code will search for both of them to look for a match. I use this in a situation where I have a wall box that is too small for a smart switch.  It would also work if you don't want to spend the cost on a smart wall switch when the only thing you want to have automated is the color temperature of the bulbs.

It is known that certain Sengled LEDs will send a signal saying they have been turned off when you kill power to them. This makes them useful for non-smart switched operations. Philips hue will send a reachback value when turned on and refreshed while being paired through their hub. Because of this they can be used without a smart switch as well.  Their may be others.
