
# API Rules
http://cinerama.gccitcom.iq/api/page/{pagenumber}/{type}/{genre}/{language}/{sort}

{pagenumber} = Page number used for pagination

{type} = Show type 0 = Movies , 1 = Series , 2 = any

{genre} = genre ID you can get it from this api call http://cinerama.gccitcom.iq/api/genry, write 0 if dont want to filter by genre

{language} = numbers from 1~9 represent show language no current api to bring all language :( , write 0 if dont want to filter by language

{sort} = "desc" and "asc" used to sort shows

# Search
you can use previous API to search for show just add /search/{searchquery} at the end like :

http://cinerama.gccitcom.iq/api/page/{pagenumber}/{type}/{genre}/{language}/{sort}/search/{searchquery}

{searchquery} = String to search for

# Seasons for Series

http://cinerama.gccitcom.iq/api/seasons/{showid} 

{showid} = Show ID you got it from main API call

# Episodes for Seasons
http://cinerama.gccitcom.iq/api/episodes/{showid}/{seasonid} 

{showid} = Show ID you can get it from main API call

{seasonid} = Season ID you can get it from Seasons API call

# Genre
http://cinerama.gccitcom.iq/api/genry

this will bring all genry with their ID

# Featured Shows
http://cinerama.gccitcom.iq/api/featured

This will bring Featured shows directly

# Slider or Pager at home screen
http://cinerama.gccitcom.iq/api/pager

this call bring shows that appears in main home slider.

# Increase View
http://cinerama.gccitcom.iq/api/counter/{episodeid}

{episodeid} = Episode ID you got it from Episodes API call used to increase views counter for episode
