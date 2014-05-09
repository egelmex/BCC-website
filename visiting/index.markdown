---
layout: map
title: Visiting
---
<link rel="stylesheet" href="http://cdn.leafletjs.com/leaflet-0.7.1/leaflet.css" />

## Getting to Canterbury ##

{% row %}
{% span 6 %}
## Train: ##

* London (St Pancras) to Canterbury West: High speed trains – journey time approximately 55 minutes. Trains depart on an hourly basis.
* London (Victoria) to Canterbury East: journey time approximately 85 minutes.
* London (Charing Cross or Waterloo East) to Canterbury West: journey time approximately 90 minutes.

{% endspan %}

{% span 6 %}
## Car: ##

* From London, the North and East Anglia (via M25 clockwise): Leave M25 at junction 2 signposted A2 Canterbury, continue on A2/M2, leave M2 at junction 7 signposted A2 Canterbury. Follow signs to Canterbury.
* From the West and South-West (via M25 anticlockwise): At M25 junction 5 continue ahead on M26(M20) signposted Maidstone, leave M20 at junction 7 signposted A249 Canterbury, join M2 at junction 5 for Canterbury, leave M2 at junction 7 signposted A2 Canterbury. Follow signs to Canterbury.
* From the South-East: Maidstone and Tonbridge: M20, A249, M2, A2 Ashford: A28 Folkestone: M20, A28 Dover: A2.
Staying in Canterbury

{% endspan %}

## Accomidation: ##

If you don’t live in Canterbury, you’re going to need somewhere to stay during BarCamp Canterbury. Unfortunately this is one thing we cannot make free, and there is no sleeping in the venue. There are, however, many reasonably-priced establishments in Canterbury. The list below should help you find somewhere to stay (we are not affiliated with any of the companies listed here and take no responsibility for the quality of your sleep).

{% endrow %}

* [kipps hostel](ttp://www.kipps-hostel.com/)
    * £16 to £20.50 for dorms
    * £22.50 to £26 for Single Rooms
    * £1.50 breakfasts
    * Group offers
* [Kent Hospitality](http://kenthospitality.kent.ac.uk/kxBnB/)
    * From £45.00
    * [canterbury.co.uk/accommodation](http://www.canterbury.co.uk/accommodation/)
* Lots of BnBs, hostels, camp-sites here.
* [Camping and caravaning](http://www.campingandcaravanningclub.co.uk/siteseekerlite/aspx/details.aspx?id=7050)
    * Camping from around £17
* Find a Canterburian to stay with! Feel free to use the comments to find people with floor space.

<script src="http://cdn.leafletjs.com/leaflet-0.7.1/leaflet.js"></script>
<script src="../assets/js/leaflet-providers.js"></script>
<script>
	var map = L.map('map').setView([51.279528, 1.087646], 13);
	var defaultLayer = L.tileLayer.provider('Stamen.Toner').addTo(map);

var myIcon = L.icon({
    iconUrl: '/assets/images/generated/barcamp4-logo-35x35-9be98f.png',
    iconSize: [32, 32],
    iconAnchor: [22, 32],
    popupAnchor: [-3, -32],
    shadowSize: [68, 32],
    shadowAnchor: [22, 32]
});

var marker_parking = L.marker([51.29945, 1.06800]).addTo(map);
marker_parking.bindPopup("<b>Parking!</b><br>It's free!");

var marker_woolf = L.marker([51.300, 1.071],{icon:myIcon}).addTo(map);
marker_woolf.bindPopup("<b>Woolf College!</b><br>The Venue.").openPopup();

</script>
