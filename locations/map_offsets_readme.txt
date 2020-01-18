MAP OFFSETS
Because each map was pulled from the master map, the coordinates of one item on the full map is an offset of the coordinates on the individual map.

These are those offsets:
CRATERIA
X: 321
Y: 0

BRINSTAR
X: 1 (oops, got the padding wrong. Not updating the full map to remove 1px from the left and then 150 item locations though)
Y: 1422

MARIDIA
X: 385
Y: 700

NORFAIR
X: 438
Y: 1854

For example, here is a Guardian Location in norfair:

{
	"name": "West Norfair Lava Guardian",
	"sections": [
	  {
		"name": "Guardian",
		"item_count": 1
	  }
	],
	"map_locations": [
	  {
		"map": "norfairmap",
		"x": 89,
		"y": 536
	  },
	  {
		"map": "fullmap",
		"x": 527, <---- 89 (location on norfair map) + 438 (offset)
		"y": 2380 <---- 536 (location on norfair map) + 1854 (offset)
	  }
	]
},