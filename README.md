# opendatahub-events-visualizations

Thir repository collects HTML files which have preconfigured views of the Webcomponents
(events-today-noi)[https://github.com/noi-techpark/webcomp-events-today-noi.git]
(events-today-eurac)[https://github.com/noi-techpark/webcomp-events-today.git]
  
This webcomponents are used by 
- NOI to display Events
- Eurac to display Events
- NOI Bruneck to display Events

## Eurac

Eurac is using this webcomponent (events-today-eurac)[https://github.com/noi-techpark/webcomp-events-today.git]

The Events of Eurac are inserted with their EBMS MeetingManagement Platform and syncronized every 15 Minutes into Open Data Hub.  
Eurac has two fields to activate/deactivate Events  
`Display1` --> Videowall Reception EURAC --> `PublishedOn: eurac-videowall` is assigned  
`Display2` --> Videowall in front of seminarrooms EURAC --> `PublishedOn: eurac-seminarroom` is assigned  
  
A Live Check on what Eurac is displaying can be found in this link `https://todayeuracedu.z6.web.core.windows.net/` + adding thename of the HTML files which are stored in the folder 'eurac'  

### Videowall

The Videowall in the Reception is AllRooms.html it shows only PublishedOn = `eurac-videowall`

### Seminarrooms

All other html files are Videowalls in front of rooms it shows only PublishedOn = `eurac-seminarroom`

## NOI 

NOI is using this webcomponent (events-today-noi)[https://github.com/noi-techpark/webcomp-events-today.git]
The Event Location Parameter is set to `eventlocation=NOI`  
  
The Events of NOI are inserted with their EBMS MeetingManagement Platform and syncronized every 15 Minutes into Open Data Hub.  
Basically there are two fields to activate/deactivate Events  
`Display3` --> NOI Totem --> `PublishedOn: noi-totem` is assigned  
`Display4` --> NOI Videowall --> `PublishedOn: today.noi.bz.it` is assigned  

Also Events are inserted manually by NOI Communication. 
Noi Communication can insert Publishers for  
`noi.bz.it` --> NOI Website active  
`noi-communityapp` --> NOI CommunityApp active  

### Special Rules
`Comment: x` Rule:  
TO EXPLAIN HERE  
`eventgrouping` Parameter:  
TO EXPLAIN HERE  

### Videowall

the link used on the Videowall is 'https://today.noi.bz.it/?location=foyer'

### Totems

The Totems have their own Api which syncs all Events from Open Data Hub each 15 Minutes.   
The api used is https://api.epaper.opendatahub.com/swagger-ui.html

## NOI Bruneck / Nobis

NOI BRUNECK is using this webcomponent (events-today-noi)[https://github.com/noi-techpark/webcomp-events-today.git]
  
The Event Location Parameter is set to `eventlocation=NOI Bruneck`  

`PublishedOn: nobis` --> indicates if the Event is active on Nobis Videowall
