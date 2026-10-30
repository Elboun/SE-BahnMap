#SE-BahnMap: Project Description
##Project Overview:
###Project vision:
Real-time web application to visualise public transport (regional/ national/ worldwide) like trains, buses, ferries (Bodensee as base example) on an interactive map (Similar to Flight Radar 24). 
Displays different data like telemetry, logs, and delay to identify chronic transportation bottlenecks.
###Problem to solve:
Existing solutions like “geOps” suffer from performance lag when handling unoptimised loads and lack comprehensive bus/ ferry data.
“Zugfinder” lacks interactive map navigation.
Official Transport Apps like “DB Navigator” often provide optimistic delay forecasts.
SE-BahnMap addresses this by visualising actual historical reliability and delay hotspots so commuters can make informed route choices.
###Technologies to use:
- Backend Ingestion: Go, Protocol Buffers, HTTP client libraries.
- Real-time communication: Go, WebSocket (gorilla/ WebSocket).
- Database & Spatial Engine (database understand latitude, longitude, lines, and polygons): PostSQL with PostGIS (PostgreSQL extension that turns database into a geographic map database), SQL migration tools.
- Frontend Map & UI: JavaScript/ TypeScript, Leaflet (JavaScript library for interactive Maps).
- Infrastructure & Integration: Docker, Docker Compose, Git/ GitHub Actions, animation loops.
###Time Frame:
10 Weeks Project: 5-member Team distributed across parallel module development and final integration phase.
##How the Soft. Engineering lecture fits in:
###Specification:
- Define clear functional requirements.
- Define clear non-functional requirements.
###Design (Software Design):
####OOP:
####UML:
- Map out class diagrams, component diagrams, and sequence diagrams showing how JSON data flows from external APIs
####Databases:
- Set up the tables.
- Relational schema.
- Set up PostGIS spatial indexing to log delay histories.
####Persistance:
####Threads:
- Handle concurrent background workers, goroutines, and safe WebSocket message broadcasting without race conditions.
####Tests:
- Apply unit API parsers, validate spatial SQL queries, and conduct WebSocket load tests.
####Process Management:
- Implement feature branch & pull request workflow to prevent merge conflicts and ensure code quality.
