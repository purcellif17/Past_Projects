# Welcome
Hello! I'm honored that you've decided to pay a visit. If you've come here from [my LinkedIn page](https://www.linkedin.com/in/ianpurcell/), you're in the right place! I've created this repository to share a bit of additional technical details of problems that I have solved in previous positions that I can't share the code for, or the code no longer meets my personal standards. With each new position or task that I take on, I learn an additional skill that I wish I had known on a previous project, so occasionally I'll resurrect an old script that has been improved enough to share with the outside world. I'm glad you've come to see some of my work, and I'm excited to share it with you!

# Introduction
My background is in Emergency Management and 9-1-1, and I got my degree in Geography and Geospatial Information Systems (GIS) from the University of Mary Washingtion. While in college, I worked as an Emergency Medical Technician for the local rescue squad. My experience working in the field as an EMT has proved invaluable at every job I have gone to, since it gives me an appreciation for exactly what someone working with the products I create would want.

# Projects, jobs, accomplishments
## Fredericksburg Fire Department, GIS Intern

During my senior year, I interned with the Fredericksburg Fire Department as a GIS intern, and produced pre-planning maps for Tier II (EPA mandated hazardous material reporting) facilities in the City of Fredericksburg. At the same time, I was finishing my GIS certificate at the University of Mary Washington, which included some programming courses. I applied some of the things I was learning in my Programming in GIS course to this project, and created a python toolbox in ArcGIS that would create a buffer around a Tier II facility based on the hazardous material evacuation recommendations in the [Emergency Response Guidebook](https://www.phmsa.dot.gov/hazmat/erg/emergency-response-guidebook-erg). The key benefit for future users was that whenever a facility updated it's reported Tier II substances, the tool could be run again.

## Dorchester County Emergency Management/9-1-1, GIS Analyst

Dorchester County Emergency Management was my first job after college. 

### Projects
#### Automating the 9-1-1 GIS Update process
One of the first projects I started was automating the data update process for our 9-1-1 system. To do so, I needed to download the appropriate feature classes from the county's GIS server and put them into a file geodatabased that matched the 9-1-1 system's schema. The entire process went from taking 4 hours for a full update to 5 minutes. 

#### Population estimator
Another tool that I built to helped save our GIS department a lot of time was a population estimator. A common question in county government is "how many people live in (fire/tax/school district)". The process beforehand was a rather manual process that involved selecting address points within a district and filtering for residential properties, then multiplying by the persons per household variable for the given area. Naturally, the people requestiong population estimates expected a rather quick answer, so a tool that would give a faster number was needed. With a district input, the population estimator tool would return the population for the given area. It helped cut a manual process from 15 minutes to 5 seconds.

#### Rebuilt county level address locators
When I worked for Dorchester County, the Charleston area was undergoing substantial growth. It felt like there was a new neighborhood every other week. This was a problem for our online web applications because people would search for their property on the web map and get no results returned because the address had not been processed yet or the building was so new that it's address was not available on the Esri geolocator. The 9-1-1 locators were more flexible than the locators on the web app because they got updated whenever a 9-1-1 update was done. The downside was that the locators were not compatable with our online system. I rebuilt the geolocators to function with both the 9-1-1 system and the county web applications, and allow both telecommunicators and citizens to search by parcel number in addition to searching by address.
