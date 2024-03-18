## SurvolFF web extension

### Description
This is a web browser extension. It adds a clickable button `survol` under the **more** menu of each flight on the foreflight dispatch page at: https://dispatch.foreflight.com \
<img width="773" alt="Capture d’écran 2024-03-12 à 09 58 12" src="https://github.com/inis17/survolFF/assets/56741837/138f4c08-6d7e-4924-b71f-979f45739ff2"> \
A click on this `survol` button starts the download of a `YYYY-MM-DD_ICAO-OACI.xlsx` file in the following format:

| Country | Fir entry point | Fir entry time | FIR entry time (UTC) | Navpoints/Route                                                 | Fir exit point | Fir exit time | FIR exit time (UTC) | FL  | TAS |
| ------- | --------------- | -------------- | -------------------- | --------------------------------------------------------------- | -------------- | ------------- | ------------------- | --- | --- |
| FRA     | LFPV            | 00:00          |                      | LGL1V LGL UN502 JSY DCT                                         | LIZAD          | 01:05         |                     | 400 | 246 |
| GBR     | LIZAD           | 01:05          |                      | DCT                                                             | ARKIL          | 01:45         |                     | 400 | 246 |
| OCC     | ARKIL           | 01:45          |                      | DCT UNLID DCT XETBO DCT | 5150N          | 08:10         |                     | 400 | 246 |
| CAN     | 5150N           | 08:10          |                      | DCT ALLRY N358A                                                 | EBONY          | 11:20         |                     | 400 | 246 |
| USA     | EBONY           | 11:20          |                      | DCT AJJAY OOSHN5                                                | KBOS           | 12:20         |                     | 400 | 246 |


This xlsx file can then be imported in the the **route** tab of an *in tasking* mission of MEAT.
### Installation
#### Firefox
Install this extension by drag and dropping the file `survolff-1.X.Y.Z.xpi` on any window of your Firefox web browser. Accept the authorisation for `public-api.foreflight.com` and `cdn.prod.foreflight.com` \
You can as well go to **about:addons** and click on the setting icon **install a module from a file**
#### Chrome
Download the extension from shared link and start using it.
#### Edge
Download the extension from shared link and start using it. \
*The edge version of the extension is similar to the Chrome one.*
### First usage
On the first usages the user will be prompt to submit a Foreflight API key. This key is requiered to access the navlogs and the routes of each flights.
You can ask your dispatch admin to generate an API key and start using the extension.
<img width="886" alt="API_console" src="https://github.com/inis17/survolFF/assets/56741837/b8b3fc52-f120-4e82-b40f-943ad41d915d">
### References
https://code7700.com/arinc_424_shorthand.htm \
https://osm-boundaries.com/ \
https://github.com/vatsimnetwork/vatspy-data-project/ \
https://eatc-mil.com/en
### Ressources
[turf.js](https://turfjs.org "Turfjs's Homepage") \
[sheet.js](https://sheetjs.com "Sheet.js' Homepage")
