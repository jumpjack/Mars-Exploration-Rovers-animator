<img width="1246" height="607" alt="image" src="https://github.com/user-attachments/assets/aac39aa1-9563-4435-8cec-893fdb61d45d" />


# Mars-Exploration-Rovers-animator
Spirit and Opportunity (MER-A and MER-B) were only able to take static images, no videos; the procedure and the web page in this repository allows  you to create smooth video transitions from static images by using stereophotogrammetry and Artificial Intelligence

## Web page
THe web pages allows loading two images, to be used as start and end frame of the video, and to manually mark them with some markers; a dozen of markers are usually enough to allow AI to match the two images and create a smooth transition. Press spave bar to toggle between pan/zoom and edit mode. Once you have placed enough markers, save the left and right images; you can also save/load the marker positions for further editing. Other buttons in the page are under test and experimental, so you can just ignore them at this moment.

## Creating the video with  AI
Go to https://app.pixverse.ai/create/transition ; upload the left and right images as start and end frame, then type one of these prompts, dependin on your specifi case:
- To get way from a location: "simulate camera motion moving  away from subject on an uneven terrain, keep consistency of color markers, keep consistency of rocks, keep consistency of terrain, remove color markers, new features enter the frame from edges, do not add moving rocks, do not add dust devils"
- To move forward: "simulate camera motion moving  forward on an uneven terrain, keep consistency of color markers, keep consistency of rocks, keep consistency of terrain, remove color markers, do not add moving rocks, do not add dust devils"
- To turn right: "turn camera to the right, some features disappear under left edge, some new features appear from right edge, keep consistency of color marker, keep consistency of terrain, keep consistency of rocks, don't add dust devils, don't add moving rocks"

If regardless of your prompt some moving rocks or dustdevils are added, it means that in that location there are not enough markers, then AI can't identify details to create a transition, so it decides to use some fantasy...

## Images repositories
- Spirit:
   - Pancam: https://planetarydata.jpl.nasa.gov/img/data/mer/spirit/mer2po_0xxx/
   - Navcam: https://planetarydata.jpl.nasa.gov/img/data/mer/spirit/mer2no_0xxx/
   - Hazard cam: https://planetarydata.jpl.nasa.gov/img/data/mer/spirit/mer2ho_0xxx/
- Opportunity:
   - Pancam: https://planetarydata.jpl.nasa.gov/img/data/mer/opportunity/mer1po_0xxx/
   - Navcam: https://planetarydata.jpl.nasa.gov/img/data/mer/opportunity/mer1no_0xxx/
   - Hazard cam: https://planetarydata.jpl.nasa.gov/img/data/mer/opportunity/mer1ho_0xxx/

