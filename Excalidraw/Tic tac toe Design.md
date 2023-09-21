---

excalidraw-plugin: parsed
tags: [excalidraw]

---
==⚠  Switch to EXCALIDRAW VIEW in the MORE OPTIONS menu of this document. ⚠==


# Text Elements
Tic-tac-toe ^rwSRcA7J

Board

- PlayerPiece[][] board ^LBJyzesD

PlayerPiece

symbol ^JlHaNhFG

Game

- Board board
- Move[] moves
- Queue players
- StatusEnum status ^6Q8Zdz6P

has a ^nzpAYLXw

Player

- String Name
- PlayerPiece peice ^FrpijKfO

Move

- Player player
- Time time
- pair position ^Zom1XGKb

has a list ^aNDRHbHa

has a ^P655odhr

has a(two) ^Qi1mtXzY

setMove(position, playerPiece) ^AxOREl9f

setter & getters
 ^HBe9LOwN

GameService ^cYHLtk3t

%%
# Drawing
```json
{
	"type": "excalidraw",
	"version": 2,
	"source": "https://github.com/zsviczian/obsidian-excalidraw-plugin/releases/tag/1.9.7",
	"elements": [
		{
			"type": "text",
			"version": 271,
			"versionNonce": 718631555,
			"isDeleted": false,
			"id": "rwSRcA7J",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -409.89843381106255,
			"y": -702.2932756025714,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 321.11395263671875,
			"height": 69.87180269681491,
			"seed": 2039429049,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693191853162,
			"link": null,
			"locked": false,
			"fontSize": 55.89744215745193,
			"fontFamily": 1,
			"text": "Tic-tac-toe",
			"rawText": "Tic-tac-toe",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Tic-tac-toe",
			"lineHeight": 1.25,
			"baseline": 48
		},
		{
			"type": "line",
			"version": 365,
			"versionNonce": 760425261,
			"isDeleted": false,
			"id": "fVvMR9B_d6fo4TeU5Cwqr",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -511.55877852134336,
			"y": -706.4662046891556,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 1.1147328361744293,
			"height": 73.20079184338395,
			"seed": 1534198201,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1693191853162,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					1.1147328361744293,
					73.20079184338395
				]
			]
		},
		{
			"type": "line",
			"version": 349,
			"versionNonce": 1697262115,
			"isDeleted": false,
			"id": "XKDvzWCy5NuTmKwBX_6zS",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -490.75045038952544,
			"y": -707.2093621812016,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 1.4863285916706612,
			"height": 74.68710002368677,
			"seed": 1313582935,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1693191853162,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					1.4863285916706612,
					74.68710002368677
				]
			]
		},
		{
			"type": "line",
			"version": 300,
			"versionNonce": 2038381965,
			"isDeleted": false,
			"id": "7rj4o5pyDMlcaxmTrsitW",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -539.0555308853651,
			"y": -681.1989248012721,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 71.71447005550257,
			"height": 3.7157806564409532,
			"seed": 1687761305,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1693191853162,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					71.71447005550257,
					-3.7157806564409532
				]
			]
		},
		{
			"type": "line",
			"version": 361,
			"versionNonce": 1330048451,
			"isDeleted": false,
			"id": "U4z42McOhVJQ8P72KEFkp",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -540.5418322618785,
			"y": -658.5326995374444,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 78.03129853221006,
			"height": 4.458931344697717,
			"seed": 579553433,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1693191853162,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					78.03129853221006,
					-4.458931344697717
				]
			]
		},
		{
			"type": "rectangle",
			"version": 444,
			"versionNonce": 1597637613,
			"isDeleted": false,
			"id": "cu2Nklw6enuVlDZGfi6Yw",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -546.3727309677629,
			"y": -715.4984218052457,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 87.6922983022837,
			"height": 92.8944075503953,
			"seed": 662991991,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1693191853162,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 354,
			"versionNonce": 2071248695,
			"isDeleted": false,
			"id": "84aCOpn_45bN8wEFUMFKO",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 311.414441697141,
			"y": -238.984138986758,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 355,
			"height": 203,
			"seed": 1458426871,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "LBJyzesD"
				},
				{
					"id": "CKn9Vf6XrdsWDkWbqs9PG",
					"type": "arrow"
				},
				{
					"id": "BJQE2zQhSpPO2YQ-lxPjj",
					"type": "arrow"
				}
			],
			"updated": 1693190013328,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 429,
			"versionNonce": 982218211,
			"isDeleted": false,
			"id": "LBJyzesD",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 372.57458268835194,
			"y": -174.984138986758,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 232.67971801757812,
			"height": 75,
			"seed": 615501721,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693191534469,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Board\n\n- PlayerPiece[][] board",
			"rawText": "Board\n\n- PlayerPiece[][] board",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "84aCOpn_45bN8wEFUMFKO",
			"originalText": "Board\n\n- PlayerPiece[][] board",
			"lineHeight": 1.25,
			"baseline": 66
		},
		{
			"type": "rectangle",
			"version": 811,
			"versionNonce": 1533621891,
			"isDeleted": false,
			"id": "fWRNzk4Daw9cjsjJryO8C",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1153.7618931361608,
			"y": -193.51967075892873,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 150,
			"height": 137,
			"seed": 655722425,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "JlHaNhFG"
				},
				{
					"id": "g_pjE8VOiml0fcpYyDK8J",
					"type": "arrow"
				},
				{
					"id": "ZecfQfsApKEKUH_buQu5c",
					"type": "arrow"
				}
			],
			"updated": 1693191696009,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 794,
			"versionNonce": 1405986605,
			"isDeleted": false,
			"id": "JlHaNhFG",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1133.8918293544225,
			"y": -162.51967075892873,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 110.25987243652344,
			"height": 75,
			"seed": 57563417,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693191696009,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "PlayerPiece\n\nsymbol",
			"rawText": "PlayerPiece\n\nsymbol",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "fWRNzk4Daw9cjsjJryO8C",
			"originalText": "PlayerPiece\n\nsymbol",
			"lineHeight": 1.25,
			"baseline": 66
		},
		{
			"type": "rectangle",
			"version": 578,
			"versionNonce": 1303985411,
			"isDeleted": false,
			"id": "Bgsqms6YClo0v8tWm7tqu",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -311.04658479611624,
			"y": -464.84750048797025,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 239,
			"height": 203,
			"seed": 300000247,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "6Q8Zdz6P"
				},
				{
					"id": "CKn9Vf6XrdsWDkWbqs9PG",
					"type": "arrow"
				},
				{
					"id": "oKc67hkrGoQsQXjBf8vyN",
					"type": "arrow"
				},
				{
					"id": "oeg8Z9c9o1ESlCDANzRS6",
					"type": "arrow"
				}
			],
			"updated": 1693191927271,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 796,
			"versionNonce": 1934051501,
			"isDeleted": false,
			"id": "6Q8Zdz6P",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -298.7464520446514,
			"y": -438.34750048797025,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 214.3997344970703,
			"height": 150,
			"seed": 1276644631,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693191927271,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Game\n\n- Board board\n- Move[] moves\n- Queue players\n- StatusEnum status",
			"rawText": "Game\n\n- Board board\n- Move[] moves\n- Queue players\n- StatusEnum status",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "Bgsqms6YClo0v8tWm7tqu",
			"originalText": "Game\n\n- Board board\n- Move[] moves\n- Queue players\n- StatusEnum status",
			"lineHeight": 1.25,
			"baseline": 141
		},
		{
			"type": "arrow",
			"version": 970,
			"versionNonce": 1981000461,
			"isDeleted": false,
			"id": "CKn9Vf6XrdsWDkWbqs9PG",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -64.33063546394112,
			"y": -323.9940370789473,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 361.3777897989213,
			"height": 117.80852575122725,
			"seed": 461435511,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "nzpAYLXw"
				}
			],
			"updated": 1693191927271,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "Bgsqms6YClo0v8tWm7tqu",
				"gap": 7.715949332175114,
				"focus": -0.016441299137951483
			},
			"endBinding": {
				"elementId": "84aCOpn_45bN8wEFUMFKO",
				"gap": 14.367287362160823,
				"focus": 0.03860938815426866
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					361.3777897989213,
					117.80852575122725
				]
			]
		},
		{
			"type": "text",
			"version": 7,
			"versionNonce": 1194252215,
			"isDeleted": false,
			"id": "nzpAYLXw",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 41.427802359518864,
			"y": -128.5190777738362,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 57.419921875,
			"height": 25,
			"seed": 1088172281,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693189523387,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "has a",
			"rawText": "has a",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "CKn9Vf6XrdsWDkWbqs9PG",
			"originalText": "has a",
			"lineHeight": 1.25,
			"baseline": 16
		},
		{
			"type": "rectangle",
			"version": 277,
			"versionNonce": 697623353,
			"isDeleted": false,
			"id": "bpgGgD6qv1xXsLXhm-zKh",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -788.5380959643663,
			"y": -235.3255351741219,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 235,
			"height": 199,
			"seed": 265372535,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "FrpijKfO"
				},
				{
					"id": "g_pjE8VOiml0fcpYyDK8J",
					"type": "arrow"
				},
				{
					"id": "oeg8Z9c9o1ESlCDANzRS6",
					"type": "arrow"
				}
			],
			"updated": 1693189523387,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 247,
			"versionNonce": 2011563555,
			"isDeleted": false,
			"id": "FrpijKfO",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -763.3579812182726,
			"y": -185.8255351741219,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 184.6397705078125,
			"height": 100,
			"seed": 1015634327,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693191534487,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Player\n\n- String Name\n- PlayerPiece peice",
			"rawText": "Player\n\n- String Name\n- PlayerPiece peice",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "bpgGgD6qv1xXsLXhm-zKh",
			"originalText": "Player\n\n- String Name\n- PlayerPiece peice",
			"lineHeight": 1.25,
			"baseline": 91
		},
		{
			"type": "rectangle",
			"version": 1296,
			"versionNonce": 1484998947,
			"isDeleted": false,
			"id": "s4u6CKsgUD7R9eleOqI_P",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -354.2091332767241,
			"y": 104.3913378216065,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 235,
			"height": 199,
			"seed": 2078466135,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "Zom1XGKb"
				},
				{
					"id": "oKc67hkrGoQsQXjBf8vyN",
					"type": "arrow"
				}
			],
			"updated": 1693191983017,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 1346,
			"versionNonce": 1527484045,
			"isDeleted": false,
			"id": "Zom1XGKb",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -309.87903989293505,
			"y": 141.3913378216065,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 146.33981323242188,
			"height": 125,
			"seed": 1869790583,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693191983017,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Move\n\n- Player player\n- Time time\n- pair position",
			"rawText": "Move\n\n- Player player\n- Time time\n- pair position",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "s4u6CKsgUD7R9eleOqI_P",
			"originalText": "Move\n\n- Player player\n- Time time\n- pair position",
			"lineHeight": 1.25,
			"baseline": 116
		},
		{
			"type": "arrow",
			"version": 2284,
			"versionNonce": 1293169901,
			"isDeleted": false,
			"id": "oKc67hkrGoQsQXjBf8vyN",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -179.51940365515208,
			"y": -245.30739515839093,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 22.445678633346063,
			"height": 333.48436007263126,
			"seed": 1658107289,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "aNDRHbHa"
				}
			],
			"updated": 1693191983017,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "Bgsqms6YClo0v8tWm7tqu",
				"gap": 16.54010532957932,
				"focus": -0.15990551411247017
			},
			"endBinding": {
				"elementId": "s4u6CKsgUD7R9eleOqI_P",
				"gap": 16.21437290736617,
				"focus": 0.21703999833753462
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					-22.445678633346063,
					333.48436007263126
				]
			]
		},
		{
			"type": "text",
			"version": 12,
			"versionNonce": 896515863,
			"isDeleted": false,
			"id": "aNDRHbHa",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -48.028974478247164,
			"y": 15.364890153724048,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 99.21986389160156,
			"height": 25,
			"seed": 2080748375,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693189523387,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "has a list",
			"rawText": "has a list",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "oKc67hkrGoQsQXjBf8vyN",
			"originalText": "has a list",
			"lineHeight": 1.25,
			"baseline": 16
		},
		{
			"type": "arrow",
			"version": 279,
			"versionNonce": 1665808781,
			"isDeleted": false,
			"id": "g_pjE8VOiml0fcpYyDK8J",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -797.8237012587301,
			"y": -138.32371987443233,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 186.1243547712054,
			"height": 5.853651042646192,
			"seed": 1091930521,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "P655odhr"
				}
			],
			"updated": 1693191696009,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "bpgGgD6qv1xXsLXhm-zKh",
				"gap": 9.285605294363677,
				"focus": 0.06427497844520928
			},
			"endBinding": {
				"elementId": "fWRNzk4Daw9cjsjJryO8C",
				"gap": 19.813837106225265,
				"focus": -0.06306181604193944
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					-186.1243547712054,
					5.853651042646192
				]
			]
		},
		{
			"type": "text",
			"version": 7,
			"versionNonce": 158712887,
			"isDeleted": false,
			"id": "P655odhr",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -846.1765858238111,
			"y": -176.30176198076265,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 57.419921875,
			"height": 25,
			"seed": 633248217,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693189523387,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "has a",
			"rawText": "has a",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "g_pjE8VOiml0fcpYyDK8J",
			"originalText": "has a",
			"lineHeight": 1.25,
			"baseline": 16
		},
		{
			"type": "arrow",
			"version": 361,
			"versionNonce": 1677986765,
			"isDeleted": false,
			"id": "oeg8Z9c9o1ESlCDANzRS6",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -322.79380062519624,
			"y": -308.3493838651764,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 223.31739617835353,
			"height": 105.14639258553524,
			"seed": 770530617,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "Qi1mtXzY"
				}
			],
			"updated": 1693191927273,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "Bgsqms6YClo0v8tWm7tqu",
				"gap": 11.747215829080005,
				"focus": 0.0449526804172545
			},
			"endBinding": {
				"elementId": "bpgGgD6qv1xXsLXhm-zKh",
				"gap": 7.426899160816561,
				"focus": -0.05526991528871852
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					-223.31739617835353,
					105.14639258553524
				]
			]
		},
		{
			"type": "text",
			"version": 12,
			"versionNonce": 884876631,
			"isDeleted": false,
			"id": "Qi1mtXzY",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -459.15490669473286,
			"y": -164.13508804800588,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 107.03987121582031,
			"height": 25,
			"seed": 1471380505,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693189523387,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "has a(two)",
			"rawText": "has a(two)",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "oeg8Z9c9o1ESlCDANzRS6",
			"originalText": "has a(two)",
			"lineHeight": 1.25,
			"baseline": 16
		},
		{
			"type": "ellipse",
			"version": 114,
			"versionNonce": 815169881,
			"isDeleted": false,
			"id": "lSrJWDGn9ZPD0r0H9ZfG-",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1134.3458370855026,
			"y": -104.6403074664268,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 31.858898215648424,
			"height": 32.582973123762486,
			"seed": 1688651033,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1693189567377,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 73,
			"versionNonce": 634704729,
			"isDeleted": false,
			"id": "-Ro_AlJnNwyIT9GRdKVnY",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1065.9980472653137,
			"y": -104.90645869153597,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 28.238576707261018,
			"height": 27.51450179914673,
			"seed": 1983472761,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1693189565310,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					28.238576707261018,
					27.51450179914673
				]
			]
		},
		{
			"type": "line",
			"version": 62,
			"versionNonce": 1830251191,
			"isDeleted": false,
			"id": "6-CffG-s-eQYZTX9CS3MS",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1067.4461970815419,
			"y": -76.66788198427518,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 29.686726523489142,
			"height": 27.5145017991467,
			"seed": 1920414679,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1693189565310,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					29.686726523489142,
					-27.5145017991467
				]
			]
		},
		{
			"type": "arrow",
			"version": 1574,
			"versionNonce": 1546207811,
			"isDeleted": false,
			"id": "BJQE2zQhSpPO2YQ-lxPjj",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 507.28595865371426,
			"y": -248.9176775788054,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 112.59324810012771,
			"height": 100.06098517498538,
			"seed": 454142521,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1693191871085,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "84aCOpn_45bN8wEFUMFKO",
				"gap": 9.933538592047398,
				"focus": 0.491080385160602
			},
			"endBinding": {
				"elementId": "AxOREl9f",
				"gap": 6.554583177005497,
				"focus": -0.010660554918959333
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					-112.59324810012771,
					-100.06098517498538
				]
			]
		},
		{
			"type": "text",
			"version": 851,
			"versionNonce": 819793571,
			"isDeleted": false,
			"id": "AxOREl9f",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 226.41456277811278,
			"y": -380.5332459307963,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 290.2796630859375,
			"height": 25,
			"seed": 1801035127,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "BJQE2zQhSpPO2YQ-lxPjj",
					"type": "arrow"
				}
			],
			"updated": 1693191871084,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "setMove(position, playerPiece)",
			"rawText": "setMove(position, playerPiece)",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "setMove(position, playerPiece)",
			"lineHeight": 1.25,
			"baseline": 16
		},
		{
			"type": "arrow",
			"version": 60,
			"versionNonce": 1313177581,
			"isDeleted": false,
			"id": "ZecfQfsApKEKUH_buQu5c",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1083.6191472314454,
			"y": -203.29441889908523,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 3.1519255642683675,
			"height": 141.59800198865642,
			"seed": 448776631,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1693191696010,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "fWRNzk4Daw9cjsjJryO8C",
				"gap": 9.774748140156532,
				"focus": -0.04160220269494666
			},
			"endBinding": {
				"elementId": "HBe9LOwN",
				"gap": 8.855797636085526,
				"focus": 0.20521820181365022
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					-3.1519255642683675,
					-141.59800198865642
				]
			]
		},
		{
			"type": "text",
			"version": 469,
			"versionNonce": 1716116375,
			"isDeleted": false,
			"id": "HBe9LOwN",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1155.8729143806127,
			"y": -403.7482185238272,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 172.27980041503906,
			"height": 50,
			"seed": 1139930071,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "ZecfQfsApKEKUH_buQu5c",
					"type": "arrow"
				}
			],
			"updated": 1693191171152,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "setter & getters\n",
			"rawText": "setter & getters\n",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "setter & getters\n",
			"lineHeight": 1.25,
			"baseline": 41
		},
		{
			"id": "dA8EXbUUNUKHg_nhiBy-5",
			"type": "rectangle",
			"x": 16.310751748586426,
			"y": -30.683580661950884,
			"width": 298,
			"height": 185,
			"angle": 0,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"seed": 2037496131,
			"version": 122,
			"versionNonce": 618365635,
			"isDeleted": false,
			"boundElements": [
				{
					"type": "text",
					"id": "cYHLtk3t"
				}
			],
			"updated": 1693191845708,
			"link": null,
			"locked": false
		},
		{
			"id": "cYHLtk3t",
			"type": "text",
			"x": 105.19081766655518,
			"y": 49.316419338049116,
			"width": 120.2398681640625,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 981908579,
			"version": 120,
			"versionNonce": 1252343533,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1693191845708,
			"link": null,
			"locked": false,
			"text": "GameService",
			"rawText": "GameService",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 16,
			"containerId": "dA8EXbUUNUKHg_nhiBy-5",
			"originalText": "GameService",
			"lineHeight": 1.25,
			"isFrameName": false
		},
		{
			"id": "tfjPkapk",
			"type": "text",
			"x": 233.47137884122003,
			"y": 132.33709717705585,
			"width": 14.239990234375,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 675195213,
			"version": 3,
			"versionNonce": 1169455629,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1693191781504,
			"link": null,
			"locked": false,
			"text": "2",
			"rawText": "2",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 16,
			"containerId": null,
			"originalText": "2",
			"lineHeight": 1.25,
			"isFrameName": false
		}
	],
	"appState": {
		"theme": "dark",
		"viewBackgroundColor": "#ffffff",
		"currentItemStrokeColor": "#1971c2",
		"currentItemBackgroundColor": "transparent",
		"currentItemFillStyle": "hachure",
		"currentItemStrokeWidth": 1,
		"currentItemStrokeStyle": "solid",
		"currentItemRoughness": 1,
		"currentItemOpacity": 100,
		"currentItemFontFamily": 1,
		"currentItemFontSize": 20,
		"currentItemTextAlign": "left",
		"currentItemStartArrowhead": null,
		"currentItemEndArrowhead": "arrow",
		"scrollX": 1206.5411229775752,
		"scrollY": 684.9396885372291,
		"zoom": {
			"value": 0.7000000000000001
		},
		"currentItemRoundness": "round",
		"gridSize": null,
		"currentStrokeOptions": null,
		"previousGridSize": null
	},
	"files": {}
}
```
%%