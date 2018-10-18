---
layout: datasets
title: "SpaceNet Roads Dataset"
sidebar: schema
---
# The SpaceNet Roads Dataset labeling guidelines:


1.	Road vectors must be drawn as a center line within 2m (7 pixels) of observed road:

    a.	The centerline of a road is defined as the centerline of the roadway. If a road has an even number of lanes, the centerline shall be drawn on the line separating lanes.  If the road has an odd number of lanes then the centerline should be drawn down the center of the middle lane.

    b.	Divided highways should have two centerlines, a centerline for each direction of traffic.  See below for the definition of a divided highway.

2.	Road vectors must be represented as a connected network to support routing.  Roads that intersect each other should share points as an intersection as instructed through OSM.  Roads that cross each other that are not connected (such as an overpass) should not share a point of connection.
3.	Roads must not bisect building footprints.
4.	Sections of a road that are a bridge or overpass must be labeled as a bridge via a Boolean flag.
5.	Divided highways must be represented as two lines with traffic direction indicated when possible.
6.	Surface type must be classified as:  paved, unpaved, or unknown.
7.	Road will be identified by type: (Motorway, Primary, Secondary, Tertiary, Residential, Unclassified, Cart Track)
8.	Number of lanes will be listed as number of lanes for each centerline as defined in rule 1.  If road has two lanes in each direction, the number of lanes shall equal 4.  If a road has 3 lanes in one direction and 2 directions in another the total number of lanes shall be 5.


## Definition of a divided highway:

A divided highway is a road that has a median or barrier that physically prevents turns across traffic.
A median can be:

    ●	Concrete
    ●	Asphalt
    ●	Green space
    ●	Dirt/unpaved road

A median is not:

    ●	Yellow hatched lines on pavement.


## Road type guidelines:
All road types were defined using the Open Street Maps taxonomy for key=highway. The below descriptions were taken from the [Open Street Maps tagging guidelines for highway](http://wiki.openstreetmap.org/wiki/Key:highway) and the [East Africa Tagging Guidelines](http://wiki.openstreetmap.org/wiki/East_Africa_Tagging_Guidelines).
1.	[motorway](http://wiki.openstreetmap.org/wiki/Tag:highway%3Dmotorway) - A restricted access major divided highway, normally with 2 or more running lanes plus emergency hard shoulder. Access onto a motorway comes exclusively through ramps (controlled access).  Equivalent to the Freeway, Autobahn, etc.
2.	[primary](http://wiki.openstreetmap.org/wiki/Tag:highway%3Dprimary) - National roads connect the most important cities/towns in a country. In most countries, these roads will usually be tarmacked and show center markings. (In South Sudan, however, primary roads might also be unpaved.)
3.	[secondary](http://wiki.openstreetmap.org/wiki/Tag:highway%3Dsecondary) – Secondary roads are the second most important roads in a country's transport system. They typically link medium-sized places. They may be paved but in in some countries they are not.
4.	[tertiary](http://wiki.openstreetmap.org/wiki/Tag:highway%3Dtertiary) - Tertiary roads are busy through roads that link smaller towns and larger villages. More often than not, these roads will be unpaved. However, this tag should be used only on roads wide enough to allow two cars to pass safely.
5.	[residential](http://wiki.openstreetmap.org/wiki/Tag:highway%3Dresidential) - Roads which serve as an access to housing, without function of connecting settlements. Often lined with housing.
6.	[unclassified](http://wiki.openstreetmap.org/wiki/Tag:highway%3Dunclassified) -The least important through roads in a country's system – i.e. minor roads of a lower classification than tertiary, but which serve a purpose other than access to properties. Often link villages and hamlets. (The word 'unclassified' is a historical artifact of the UK road system and does not mean that the classification is unknown; you can use highway=road for that.)
7.	Cart track – This is a dirt path that shows vehicle traffic that is less defined than a residential

Additional information and rules for road identification come from following sources:

  1) [Highway Tag Africa](http://wiki.openstreetmap.org/wiki/Highway_Tag_Africa)
  2) [East Africa Tagging Guidelines](http://wiki.openstreetmap.org/wiki/East_Africa_Tagging_Guidelines)
  3) [Key:highway](http://wiki.openstreetmap.org/wiki/Key:highway)


## GeoJSON Schema
#### Attributes:
1)	“geometry”: Linestring

2)	“road_id”: int
Identifier Index

3)	“road_type”: int

    1: Motorway
    2: Primary
    3: Secondary
    4: Tertiary
    5: Residential
    6: Unclassified
    7: Cart track

4)	“paved”: int

    1: Paved
    2: Unpaved
    3: Unknown

5)	“bridge_typ”: int

    1: Bridge
    2: Not a bridge
    3: Unknown

6)	“lane_number”: int

    1: one lane
    2: two lanes
    3: three lanes
    etc.
