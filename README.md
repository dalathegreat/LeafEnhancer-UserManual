# LeafEnhancer - User Manual
User manual for the LeafEnhancer software developed by Dala's EV Repair LeafEnhancer is a compilation of enhancements for the 2010-2017 Nissan Leaf. It brings some well needed quality of life improvements to make the older LEAF more competetive, compared to the features present on todays EVs. Here is all the enhancements:

## CapacityBoost ❌ (Work in progress)
This software allows for more extraction of usable power from the battery. This is done by tapping into the buffer that is normally used to prevent degradation. An 8% capacity increase is extracted this way. This roughly translates to 5-15km of additional range depending on your batteries current state of health.

Technically this is done by charging the cells to 4.20V, instead of the default 4.12V. Be aware that the battery degradation can be sped up if the car is left at 100% state of charge for extended periods of time with this modification. If possible, try to only charge to 100% when really needed, and use the 80% charge limiter or BatterySaver for daily use.

## BatterySaver ✔️
BatterySaver is a fully customizable maximum charge limiter, extending on the one that was originally shipped with 2011-2013 LEAFs. The stock limiter only allowed setting two limiters, 80 and 100%. The BatterySaver extends on this, and can set the max charge percentage in six steps, 50, 58, 66, 75, 83, 92, 100 %.
### Why do I need a maximum charge limiter?
To preserve battery life. By not charging the battery fully, you avoid long term battery degradation. Lithium batteries degrade faster when they are sitting at high voltages. The lower you get your discharge cycles, the better the battery will perform long term. For example much better to stay between 20-80% than it is to be at 0-100%.
### How to set the BatterySaver limit?
See this youtube video for a step by step guide: https://www.youtube.com/watch?v=yJvrB6aw5Ys
To set the charge limiter, turn on re-circulation, and set fan speed to max (7). You'll see the dash capacity bars start to move, along with the state of charge %. When the desired charge max % is reached, it can be set by turning down the fan speed.

## Glide in Drive ✔️
When enabled, 'Glide in Drive' removes regenerative braking. This can be useful for hypermiling (avoid regen on highway, it's only 80% effective) or when doing service to friction brakes, and you want to check for noise/evenness (hard when regen takes over).

Glide in drive can be enabled by shifting from D->N. After this shift, the D mode will have no regenerative braking. You will get a visual confirmation on the dashboard when you enter this mode, the outer capacity bars will momentarily only show 2 bars. To re-enable the regenerative braking, simply do another D->N shift. The capacity bars will display as 3x when the mode is exited.

For 2011-2013 ZE0 LEAF;
Glide in drive works amazingly! When you are in the glide in drive mode, you can quickly switch between D(no regen) and ECO(regen) to make driving easier. It is quite different to drive a Leaf with no regen!

For 2014-2017 AZE0 LEAF;
Glide in drive works OK-ish! When you enter glide in drive, it takes 10-30sec for the vehicle to acknowledge that the car should not regen. This makes switching between D and B very slow. There is no currently known way to speed this up.

For 2018-2020 ZE1 LEAF;
Glide in drive works, barely! Even though regen is disabled, the vehicle ignores this and continues to allow for a small amount of regen. The amount of regen is heavily reduced, but there is still some present, making for a not-so glide in drive experience.

### A word of caution
This is an extreme hypermiling mod. Glide in drive will make your vehicle rely entirely on the friction brakepads, just as a regular car. The car will slow down extremely little when you let off the accelerator pedal. This can be quite a shock for some drivers, so be prepared. Dala's EV Repair cannot be held responsible for any dangerous situations/damages caused by using this feature.

## NagscreenRemover ❌ (Work in progress)
On the 2013-2017 LEAF, it is possible to bypass the nagscreen that appears on the infotainment system when you start the vehicle. The LeafEnhancer software can take you straight to the Radio / Status screen on bootup instead of that screen.

NagscreenRemover is still being developed

## CurrentControl ❌ (Work in progress)
Adjusting AC max charge speed is something that most EV makers have on their vehicles. This setting is ofter accessed via a touchscreen inside the vehicle. Unfortunately, the Nissan Leaf is not equipped with this setting, even though the on-board-charger is technically able to decide what amount of power can go into the battery. This has led owners of the Leaf to rely on the EVSE to set the correct max power lever. Often leading to the user having to opt for a more expenive EVSE that has some current control on the cable/handle. The code here aims to correct this, and enable setting the charge speed from within the vehicle.

### How to use CurrentControl and set a max kW limiter
When the car is connected to an EVSE and is slowcharging, turn on the car to wake up the HVAC controls. Set the fan to maximum speed(7), and switch on recirculation mode. You will see the capacity bars on the dash board start to move, along with the SOC% if you have the newer LEAF that has this. These are the current options Condition held:
* under 4s equals to Unrestricted kW, Visualized as 12 capacity bars and SOC%=66
* over 4s equals to 6.0 kW, Visualized as 11 capacity bars and SOC%=60
* over 6s equals to 5.0 kW, Visualized as 10 capacity bars and SOC%=50
* over 8s equals to 4.0 kW, Visualized as 9 capacity bars and SOC%=40
* over 10s equals to 3.0 kW, Visualized as 8 capacity bars and SOC%=30
* over 12s equals to 2.0 kW, Visualized as 7 capacity bars and SOC%=20
* over 14s equals to 1.0 kW, Visualized as 6 capacity bars and SOC%=10

Use this video as a guide https://www.youtube.com/watch?v=u6fHHyJBMu8
