# Weekly Carbon Footprint Calculator
This is a weekly carbon footprint calculator that I did with my classmates in one of my computer science classes. Everything is done using the MIPS assembly language. *Below this text, all content comes from our slides.*

## Overview
- The Weekly Carbon Footprint Tracker lets users log daily activities (transport, energy, and waste) and calculates their weekly carbon footprint. It then projects this total over a year and compares it to the US average.
- This lines up with UN SDG: Goal 11 – Sustainable Cities and Communities.
- Goal Impact: Helps users understand and reduce their carbon footprint, promoting sustainable living habits.

## Targeted Users
- Users: Urban and suburban residents interested in sustainability.
- Scope: Household level, with potential for broader community impact.

## Walkthrough
1. Start
2. Ask Question (e.g., "How do you commute to work?")
3. User Input (e.g., "Bus/Public Transit")
4. Calculate Emissions for Answer
5. Update Bar Graph Dynamically (Transportation, Energy, Waste, Total Emissions)
6. Is All Input Completed? If yes then calculate Total Weekly Emissions. If no then next question and repeat
7. Project Annual Emissions
8. Trigger Audio Feedback:
   - <50% of Target: celebratory sound
   - 50%-<100%: less celebratory sound
   - 100% and greater: Warning sound
9. Compare Emissions with US average
10. Display Final Bar Graph
11. Provide Feedback
12. End

## Very Simplified Flowchart
<img width="717" height="846" alt="image" src="https://github.com/user-attachments/assets/f68c1d8a-a236-4792-be13-e421478c1b2a"/>

## Contributions
- Classmate - Research(finding equations and facts)/ File requirements /Calculations(Wrote half of the calculation files to get the emissions)/Sound
- Andy Quach (me) - Graphics(Made the bar graphs that move based on calculations)/Sound
- Classnate - Calculations(Wrote half of the calculation files to get the emissions) 

## Pitfalls
- Most of the project is very dependent on the previous person’s work, for example, the calculations needed to be done first because the graphics move and the way they move depend on the calculations.
- Work and other classes often got in the way and we could only talk during class and late at night.
- Often not everyone in the group was in class.
- Not all of our computers have the same abilities (like good sound chips and processing power) so some people could do things with no problem and others could not.
- In order to organize the code better we separated some of the functions into different asm files and assembled all files in the directory. We also had some miscommunications from time to time.
- It’s really hard to properly communicate ideas through messages, which was our primary way to talk.
- We did not have as many outside user testing as we would have liked.
- Our graphics were overwriting the data, and we fixed that by moving the display to a different location.

## Possible Improvements
- More detailed calculations: The calculations used assumes ideal conditions like no traffic for the transportation questions and no consideration of cost.
- More questions: More questions would make it so we have a bigger dataset which would make the calculations more accurate.

### --- End of Slides ---

## How To Run This Program
1. Download [MARS](https://github.com/dpetersanderson/MARS/releases/tag/v.4.5.1) (requires Java Runtime, you can download it [here](https://www.java.com/en/download/))
2. Clone this repository or download it as a ZIP file. (Make sure to rename the folder to `team-projects-fall-2024-skyliners`)
3. Make sure that MARS and the program folder are in the same directory. (For example, put `Mars4_5.jar` and the `team-projects-fall-2024-skyliners` folder in the desktop folder)
4. Open MARS.
5. Open `main.asm` in the project folder.
6. Go to `Tools > Bitmap Display` to set up the program's display.
7. Configure the display with these properties:
   - Unit width: 4
   - Unit height: 4
   - Display width: 256
   - Display height: 256
   - Base address: 0x10000000 (global data)
8. Assemble the program. (Make sure that `Assemble all files in directory` is checked)
9. The program should start running in the console window.
10. Follow the walkthrough.
