# printer-network-troubleshooting
A write up of my troubleshooting process as I fixed a printer that wasn't functioning properly.

**TLDR**: My apartment building's printer wasn't functioning: incorrect language and wouldn't print. I checked for physical obstruction, cleared printer queue, connected both devices to the same router, then the same network, and re-established connection between them to restore printing ability.

## The Problem / Context 
- I wanted to use my apartment building's printer to print a document, but it failed with no response.

## The Baseline
- First, I changed the language of the printer so I could properly navigate.
- I investigated a potential paper jam, physical obstruction, or ink shortage, which were all non-issues.

## Step 1: Checking the Queue
- I checked the printer queue via Devices & printers.
- Cleared the long queue, and tried to print again, but it failed another time.

## Step 2: Checking computer-printer Connectivity
- I realized that because the computer and printer were not physically connected, connectivity must take place over a *shared* network.
- The computer was online, but when I checked the printer, it was *offline*.

## Step 3: Connect the Printer to the Same Network
- Since the printer was connected via Ethernet, I checked for a defective cable.
- It was functioning (steady green light, flashing amber light), but was not directly connected to the same router as the computer.
- To be sure, I plugged the Ethernet cable into the same router.
- An IP address appeared. Assuming it was connected to the same network, i tried to print but failed again.

## Step 4: Both are Connected to the Same Router.. Now What?
- To make sure it wasn't a router issue, I swapped the ports of the computer and printer. No change.
- I then realized that the printer's IP address was strange. I knew for them to be on the same network, they should be similar.
- I checked the Computer's IP address, and it did not match the printer's.
- After doing some research, I learned that the printer's address was a AIPIA address, but the issue was unlikely be the router because the computer connected to the internet just fine.

## Step 5: Fix the IP Address
- I opted to reset the printer (leaving it unplugged for at least 30 seconds), but when it powered back on, the AIPIA address was still there.
- From here I looked for a way to factory reset in settings.
- Assuming that someone had been messing with the printer beforehand (Language changed, no longer functioning), I decided to reset to default settings.
- After this, the computer rebooted with the correct IP address.

## The final step
- Now that I knew both devices were connected to the same network, I searched for the printer on the computer and connected successfully.
- With a successful connection, printer functionality was restored. 

# What I learned / Final Thoughts:
- The main thing that I learned, was what an AIPIA address was. Initially I hadn't known, which led me to assume the IP address was valid.
- I learned about the role of resetting devices for some changes to take place.
- And I continued to strengthen my troubleshooting and problem solving skills.
