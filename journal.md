
# Autonomous Beach Rescue Drone

## The Idea
Simply put: Create a prototype for an autonomous drone, that would be able to provide key first-aid rescue across Australia.

## The Current Situation
Australia's extensive coastline is both a national treasure and a significant public safety challenge. The coastline is understandably a popular location for recreation, being a gem of the world. Despite the efforts of Surf Life Saving (SLS) services, many areas remain unmonitored or difficult to patrol. During the 2024-2025 summer period (December to February), **51 coastal drowning deaths** were recorded.

Alarmingly:
- 65% of these drownings occurred more than 1 km away from a patrolled SLS service

- 40% were rip-related beach drownings, with

	-	27% of those involving bystanders attempting to rescue others.

- 60% occurred in regional or rural locations.

These statistics highlight a critical need for an initial rapid-response systems in unpatrolled and remote areas. Response in these areas is currently not feasible with traditional person-based approaches due to a lack of trained people available consistently, and a low amount of people on each beach.

To address this, there is an opportunity to develop an autonomous drone system which could be deployed as part of a system across **every Australian beach**. Especially targeting high-risk and unpatrolled zones.

## What Already Exists
Well.. not much.. really. 

Currently, there exists a solution which is deployed across the country, in which under human control, and deployment, drones are able to make rescues at major beaches. This has proven very effective. Yet, it still leaves a wide part of the country unprotected (60%), thus the need for an autonomous solution arises.

The current solution also allows for shark detection.

![These Drones Are Saving Lives in Australia's Oceans | Hive Life Magazine](https://hivelife.com/wp-content/uploads/2019/12/Westpac-Little-Ripper-life-saving-drones-Hive-Life-banner.jpg)

*Current drone in place at some major Australian beaches, at some times*

## Scope of the Project
**Design and Produce:**
- A mid sized drone (5-7"), based off the FPV framework.
	- The drone is capable of autonomous flight, to a pre-specified location, when directed.
- A solution to allow for the aerial drop of a commercially available inflatable floatation system
- A solution to allow the drone to be weather-proof and protected when not in flight.

**What will *NOT* be included in this scope, yet could be next :**
- Live Rescue tests
- Autonomous vision to detect people in need of assistance.
- Recharging while stored
*This was list was come to in order to ensure safety, and also make the project achievable in under 3 months*

### Time Spent - 2 Hours (27/05/25)

---

## Design - Start of the Dock
At beaches, conditions can become unpredictable, thus it is important to ensure that the drone will be able to be stored and protected during all weather conditions, especially where in rural areas in which regular interval maintenance is not feasible. However, this does not mean/make it realistic that this solution would be able to deploy in extreme weather conditions.

![Naughty little girl threatens our summer fun | The Australian](https://content.api.news/v3/images/bin/0173e5e3decd0f2806f2c0284e900b15)
*Extreme weather on Australian Beaches*

---
Thus, I think it'll be crucial to have a dock/station where the drone is able to rest, ready to deploy when needed.

**Requirements:**
- Weatherproof
- Facilitate accurate landing
- Cheap!
	- This drone has the ambition of being deployed in mass, thus price is an important factor.

**With this, some possible implementations:**
- Weatherproof
	- Closing lid
	- Storage drawer
- Facilitate accurate landing
	- Feedback to the drone
	- Use of AprilTags to help drone determine position

---
### What's Already on the Market

Something I firmly believe in is the analysis of existing products and solutions. This can often be overlooked.

Chances be it, most ideas have probably been explored and conceptualised in some form, thus having a good understanding of what has been done allows for an extra layer of innovation, in order to make a meaningful impact on the target market and consumers of the product.

---
**DJI Dock 1**
![DJI Dock in Australia - FlytBase](https://cdn.prod.website-files.com/6336f32fe0e46462713ad519/635a291060cca8396a6ee14e_DJI-Dock1.png)

> DJI's first generation of drone dock for autonomous deployment.

**✅ Advantages**
- Rugged and durable
- Lid swings open to provide a large landing area
- Secure - has security and sensors

**❌ Disadvantages**
- Expensive :)
- Landing accuracy relies on sensors in drone
	- Not practical for my application
- Requires an external power source to operate


---
 
**DJI Dock 2**
![DJI DOCK 2 With DJI Matrice 3DT - Africa Drone Kings | DJI Drone](https://enterprise.africadroneking.co.za/wp-content/uploads/2024/03/DJIDock2_with_M3DT__1_-removebg-preview.png)

> Yeah.. so DJI is kinda popular. 


**✅ Advantages**
- Passive entering mechanism relies alot less on drone sensors to get it in
	- This is really cool
- Lid swings open using (by the looks of it) linear actuators, providing a simple, yet robust way of maximising the landing area, while using a very simple pivot mechanism.
**❌ Disadvantages**
- Expensive :)
- Landing accuracy relies on the drone - DJI has some pretty cool tech that allows this
	- Once again not feasible for my purposes.
- Requires an external power source to operate


---
**Energy Robotics Drone-in-a-box**
![Image-Remove-Background](https://i.ibb.co/XZmDXNqD/Image-Remove-Background.png)

> AprilTags are pretty cool

**✅ Advantages**
- The April tags allow for very precise landings without requiring complex sensors
- Small (this is also a disadvantage)
- Sliding drawer improves safety during rain.

**❌ Disadvantages**
- Small. Could get covered over with debris is heavy weather
	- Landing pad size gives a big constraint.
- Seems like a less robust solution compared to DJI

---

**💡 Opportunities and What Worked Well**
- All solutions require an external power-source
	- Solar Charging to allow remote deployment
- The DJI passive centring is very neat, and a good solution to allow for reduced landing accuracy
- AprilTags seem like a good way to help the drone locate itself relative to the station.
- I think the fold out design appeal more at the moment, especially considering the terrain of the beach.

---
**Block CAD!!!**
Another thing which I see as really important is the use of Block CAD to help gain sense of key mechanism parts, and it really helps to plan a design solution. 

The goal here is to keep everything **as simple as possible**.

**Initial Concept - Heavily DJI Dock 2 Based**

I thought that the DJI Dock 2 provided a very succinct solution to the problem, and the concepts could provide very successful for my project.

![image](https://i.ibb.co/cKyrgfc8/image.png)

The folding doors allow for a clear open space for the drone to take up out of, while then being able to fold in for a compact and succinct solution.

Additionally, the elevation of it allows for the potentially harsh conditions, and prevents it from getting covered and unable to open by sand or debris.

![image](https://i.ibb.co/Fq8QnzsF/image.png)

One thing I noticed from the DJI dock was how the indexing funnel was only on one side, and thus looked at implementing it I decided to experiment a bit with adding another flange on the other side. This would mean that there would be quite a large allowable margin for error when designing the landing system. This is a good thing!! It needs to work 100% of the time.

![image](https://i.ibb.co/pvZ1bZCz/image.png)

I feel like this concept has the ability to be pretty successful, and tomorrow I will look at trying something completely new involving sliding doors, just to get a sense of options.

I'm however cautious to design too much of the dock before the drone, as priorities will likely shift as the design of the drone (centre piece) evolves. It made sense to lay some groundwork for the dock first though.

**A final thought:**
Manufacturing.. oh yeah, this probably shouldn't be a final thought. Is anything on Day 2 a final thought though.. :)
I think it makes sense to try and utilise 3D printing as much as possible for this design, seeing as I'm aiming to keep the costs low for a small-quantity prototype. Industrial manufacturing process such as injection moulding don't make sense at small scale. 

Something interesting could be a aluminium frame on the inside to help with rigidity, this could be explored at a later time, once the design is more defined.


### Time Spent - 2 Hours (28/05/25)

---

## Day 2 - Further Dock Iterations 

The main goal for the dock mechanism is to be able to fold out in order to allow the drone to both take off, and land in a safe and accurate way, while also shielding it from the elements when not in use.

I identified another method of shutting the doors at the top, and rather than pivoting, have them side out of the way, like an opening hangar.

![image](https://i.ibb.co/MDkbQdtN/image.png)

To accomplish this, I first took the base from the previous design, but the first thing I had to alter was the sides.

Seeing as the doors would be sliding out of the way, it would have to be fully enclosed from all sides. To do this, I raised all sides upto the same level.

![image](https://i.ibb.co/G3nTD291/image.png)

![image](https://i.ibb.co/Vp9GyZqJ/image.png)

I came up with something like this, using similar shaped doors as the previous model, but having them slide out of the way. Unfortunately, I don't think this option has much practical validity.

![image](https://i.ibb.co/fz8tyb8X/image.png)

The doors could become quite heavy, which will come with the challenge of.. gravity. As the doors slide further out, the more force will be exerted on the mechanism that is holding it in place, to solve this, more overlap would be needed, yet this will reduce the amount of space the drone has to land in. I don't view this as an acceptable solution to the problem, harming the rigidity of the system.

Overall, I will not be pursing the sliding door archetype further, and will possibly look into some other solutions later down the track. Time to start the drone now!

### Time Spent - 2 Hours (30/05/25)
