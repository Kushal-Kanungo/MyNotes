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

%%
# Drawing
```json
{
	"type": "excalidraw",
	"version": 2,
	"source": "https://github.com/zsviczian/obsidian-excalidraw-plugin/releases/tag/1.9.7",
	"elements": [
		{
			"id": "rwSRcA7J",
			"type": "text",
			"x": -500.5268343411965,
			"y": -484.1526571420524,
			"width": 321.19976806640625,
			"height": 69.87180269681491,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 2039429049,
			"version": 217,
			"versionNonce": 219643161,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1693189523386,
			"link": null,
			"locked": false,
			"text": "Tic-tac-toe",
			"rawText": "Tic-tac-toe",
			"fontSize": 55.89744215745193,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 48,
			"containerId": null,
			"originalText": "Tic-tac-toe",
			"lineHeight": 1.25,
			"isFrameName": false
		},
		{
			"id": "fVvMR9B_d6fo4TeU5Cwqr",
			"type": "line",
			"x": -602.1871790514773,
			"y": -488.32558622863667,
			"width": 1.1147328361744293,
			"height": 73.20079184338395,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"seed": 1534198201,
			"version": 311,
			"versionNonce": 268254455,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1693189523386,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1.1147328361744293,
					73.20079184338395
				]
			],
			"lastCommittedPoint": null,
			"startBinding": null,
			"endBinding": null,
			"startArrowhead": null,
			"endArrowhead": null
		},
		{
			"id": "XKDvzWCy5NuTmKwBX_6zS",
			"type": "line",
			"x": -581.3788509196594,
			"y": -489.0687437206827,
			"width": 1.4863285916706612,
			"height": 74.68710002368677,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"seed": 1313582935,
			"version": 295,
			"versionNonce": 1731883513,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1693189523386,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1.4863285916706612,
					74.68710002368677
				]
			],
			"lastCommittedPoint": null,
			"startBinding": null,
			"endBinding": null,
			"startArrowhead": null,
			"endArrowhead": null
		},
		{
			"id": "7rj4o5pyDMlcaxmTrsitW",
			"type": "line",
			"x": -629.683931415499,
			"y": -463.0583063407532,
			"width": 71.71447005550257,
			"height": 3.7157806564409532,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"seed": 1687761305,
			"version": 246,
			"versionNonce": 358123031,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1693189523386,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					71.71447005550257,
					-3.7157806564409532
				]
			],
			"lastCommittedPoint": null,
			"startBinding": null,
			"endBinding": null,
			"startArrowhead": null,
			"endArrowhead": null
		},
		{
			"id": "U4z42McOhVJQ8P72KEFkp",
			"type": "line",
			"x": -631.1702327920125,
			"y": -440.3920810769255,
			"width": 78.03129853221006,
			"height": 4.458931344697717,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"seed": 579553433,
			"version": 307,
			"versionNonce": 1860946649,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1693189523387,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					78.03129853221006,
					-4.458931344697717
				]
			],
			"lastCommittedPoint": null,
			"startBinding": null,
			"endBinding": null,
			"startArrowhead": null,
			"endArrowhead": null
		},
		{
			"id": "cu2Nklw6enuVlDZGfi6Yw",
			"type": "rectangle",
			"x": -637.0011314978968,
			"y": -497.3578033447268,
			"width": 87.6922983022837,
			"height": 92.8944075503953,
			"angle": 0,
			"strokeColor": "#1e1e1e",
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
			"seed": 662991991,
			"version": 390,
			"versionNonce": 514698039,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1693189523387,
			"link": null,
			"locked": false
		},
		{
			"id": "84aCOpn_45bN8wEFUMFKO",
			"type": "rectangle",
			"x": 311.414441697141,
			"y": -238.984138986758,
			"width": 355,
			"height": 203,
			"angle": 0,
			"strokeColor": "#1e1e1e",
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
			"seed": 1458426871,
			"version": 354,
			"versionNonce": 2071248695,
			"isDeleted": false,
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
			"id": "LBJyzesD",
			"type": "text",
			"x": 372.57453691198475,
			"y": -174.984138986758,
			"width": 232.6798095703125,
			"height": 75,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 615501721,
			"version": 427,
			"versionNonce": 582218073,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1693189928812,
			"link": null,
			"locked": false,
			"text": "Board\n\n- PlayerPiece[][] board",
			"rawText": "Board\n\n- PlayerPiece[][] board",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 68,
			"containerId": "84aCOpn_45bN8wEFUMFKO",
			"originalText": "Board\n\n- PlayerPiece[][] board",
			"lineHeight": 1.25,
			"isFrameName": false
		},
		{
			"id": "fWRNzk4Daw9cjsjJryO8C",
			"type": "rectangle",
			"x": -1156.92333984375,
			"y": -208.27313232421892,
			"width": 150,
			"height": 137,
			"angle": 0,
			"strokeColor": "#1e1e1e",
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
			"seed": 655722425,
			"version": 791,
			"versionNonce": 966220633,
			"isDeleted": false,
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
			"updated": 1693191147589,
			"link": null,
			"locked": false
		},
		{
			"id": "JlHaNhFG",
			"type": "text",
			"x": -1137.0532836914062,
			"y": -177.27313232421892,
			"width": 110.2598876953125,
			"height": 75,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 57563417,
			"version": 772,
			"versionNonce": 1353231351,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1693189559306,
			"link": null,
			"locked": false,
			"text": "PlayerPiece\n\nsymbol",
			"rawText": "PlayerPiece\n\nsymbol",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 68,
			"containerId": "fWRNzk4Daw9cjsjJryO8C",
			"originalText": "PlayerPiece\n\nsymbol",
			"lineHeight": 1.25,
			"isFrameName": false
		},
		{
			"type": "rectangle",
			"version": 489,
			"versionNonce": 1752929495,
			"isDeleted": false,
			"id": "Bgsqms6YClo0v8tWm7tqu",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -296.29316682736635,
			"y": -240.3839559148675,
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
			"updated": 1693189972628,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 705,
			"versionNonce": 107977977,
			"isDeleted": false,
			"id": "6Q8Zdz6P",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -283.99307222287416,
			"y": -213.8839559148675,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 214.39981079101562,
			"height": 150,
			"seed": 1276644631,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693189972629,
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
			"baseline": 143
		},
		{
			"id": "CKn9Vf6XrdsWDkWbqs9PG",
			"type": "arrow",
			"x": -49.577217495191235,
			"y": -140.71895468787795,
			"width": 346.6243718301714,
			"height": 0.4459872014008397,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"seed": 461435511,
			"version": 780,
			"versionNonce": 469180599,
			"isDeleted": false,
			"boundElements": [
				{
					"type": "text",
					"id": "nzpAYLXw"
				}
			],
			"updated": 1693190010253,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					346.6243718301714,
					-0.4459872014008397
				]
			],
			"lastCommittedPoint": null,
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
			"startArrowhead": null,
			"endArrowhead": "arrow"
		},
		{
			"id": "nzpAYLXw",
			"type": "text",
			"x": 41.427802359518864,
			"y": -128.5190777738362,
			"width": 57.41996765136719,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1088172281,
			"version": 7,
			"versionNonce": 1194252215,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1693189523387,
			"link": null,
			"locked": false,
			"text": "has a",
			"rawText": "has a",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 18,
			"containerId": "CKn9Vf6XrdsWDkWbqs9PG",
			"originalText": "has a",
			"lineHeight": 1.25,
			"isFrameName": false
		},
		{
			"id": "bpgGgD6qv1xXsLXhm-zKh",
			"type": "rectangle",
			"x": -788.5380959643663,
			"y": -235.3255351741219,
			"width": 235,
			"height": 199,
			"angle": 0,
			"strokeColor": "#1e1e1e",
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
			"seed": 265372535,
			"version": 277,
			"versionNonce": 697623353,
			"isDeleted": false,
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
			"id": "FrpijKfO",
			"type": "text",
			"x": -763.3580041064562,
			"y": -185.8255351741219,
			"width": 184.6398162841797,
			"height": 100,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1015634327,
			"version": 245,
			"versionNonce": 1277300695,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1693191132939,
			"link": null,
			"locked": false,
			"text": "Player\n\n- String Name\n- PlayerPiece peice",
			"rawText": "Player\n\n- String Name\n- PlayerPiece peice",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 93,
			"containerId": "bpgGgD6qv1xXsLXhm-zKh",
			"originalText": "Player\n\n- String Name\n- PlayerPiece peice",
			"lineHeight": 1.25,
			"isFrameName": false
		},
		{
			"type": "rectangle",
			"version": 1272,
			"versionNonce": 1383281465,
			"isDeleted": false,
			"id": "s4u6CKsgUD7R9eleOqI_P",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -298.3567337231527,
			"y": 131.7907170068744,
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
			"updated": 1693189974479,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 1320,
			"versionNonce": 670529751,
			"isDeleted": false,
			"id": "Zom1XGKb",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -254.02667085694173,
			"y": 168.7907170068744,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 146.33987426757812,
			"height": 125,
			"seed": 1869790583,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693189974479,
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
			"baseline": 118
		},
		{
			"id": "oKc67hkrGoQsQXjBf8vyN",
			"type": "arrow",
			"x": -156.38680564473958,
			"y": -20.843850585288173,
			"width": 0.610840926074701,
			"height": 136.4201946847964,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"seed": 1658107289,
			"version": 2044,
			"versionNonce": 1314932215,
			"isDeleted": false,
			"boundElements": [
				{
					"type": "text",
					"id": "aNDRHbHa"
				}
			],
			"updated": 1693189974479,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.610840926074701,
					136.4201946847964
				]
			],
			"lastCommittedPoint": null,
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
			"startArrowhead": null,
			"endArrowhead": "arrow"
		},
		{
			"id": "aNDRHbHa",
			"type": "text",
			"x": -48.028974478247164,
			"y": 15.364890153724048,
			"width": 99.21992492675781,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 2080748375,
			"version": 12,
			"versionNonce": 896515863,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1693189523387,
			"link": null,
			"locked": false,
			"text": "has a list",
			"rawText": "has a list",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 18,
			"containerId": "oKc67hkrGoQsQXjBf8vyN",
			"originalText": "has a list",
			"lineHeight": 1.25,
			"isFrameName": false
		},
		{
			"id": "g_pjE8VOiml0fcpYyDK8J",
			"type": "arrow",
			"x": -797.8237012587301,
			"y": -142.82797082696555,
			"width": 189.2858014787946,
			"height": 0.8570241308808022,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"seed": 1091930521,
			"version": 233,
			"versionNonce": 547598841,
			"isDeleted": false,
			"boundElements": [
				{
					"type": "text",
					"id": "P655odhr"
				}
			],
			"updated": 1693191133878,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-189.2858014787946,
					-0.8570241308808022
				]
			],
			"lastCommittedPoint": null,
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
			"startArrowhead": null,
			"endArrowhead": "arrow"
		},
		{
			"id": "P655odhr",
			"type": "text",
			"x": -846.1765858238111,
			"y": -176.30176198076265,
			"width": 57.41996765136719,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 633248217,
			"version": 7,
			"versionNonce": 158712887,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1693189523387,
			"link": null,
			"locked": false,
			"text": "has a",
			"rawText": "has a",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 18,
			"containerId": "g_pjE8VOiml0fcpYyDK8J",
			"originalText": "has a",
			"lineHeight": 1.25,
			"isFrameName": false
		},
		{
			"id": "oeg8Z9c9o1ESlCDANzRS6",
			"type": "arrow",
			"x": -308.04038265644635,
			"y": -142.90736496035106,
			"width": 238.07081414710342,
			"height": 1.0196181776943263,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"seed": 770530617,
			"version": 171,
			"versionNonce": 690817753,
			"isDeleted": false,
			"boundElements": [
				{
					"type": "text",
					"id": "Qi1mtXzY"
				}
			],
			"updated": 1693191133878,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-238.07081414710342,
					1.0196181776943263
				]
			],
			"lastCommittedPoint": null,
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
			"startArrowhead": null,
			"endArrowhead": "arrow"
		},
		{
			"id": "Qi1mtXzY",
			"type": "text",
			"x": -459.15490669473286,
			"y": -164.13508804800588,
			"width": 107.0399169921875,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1471380505,
			"version": 12,
			"versionNonce": 884876631,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1693189523387,
			"link": null,
			"locked": false,
			"text": "has a(two)",
			"rawText": "has a(two)",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 18,
			"containerId": "oeg8Z9c9o1ESlCDANzRS6",
			"originalText": "has a(two)",
			"lineHeight": 1.25,
			"isFrameName": false
		},
		{
			"id": "lSrJWDGn9ZPD0r0H9ZfG-",
			"type": "ellipse",
			"x": -1134.3458370855026,
			"y": -104.6403074664268,
			"width": 31.858898215648424,
			"height": 32.582973123762486,
			"angle": 0,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"seed": 1688651033,
			"version": 114,
			"versionNonce": 815169881,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1693189567377,
			"link": null,
			"locked": false
		},
		{
			"id": "-Ro_AlJnNwyIT9GRdKVnY",
			"type": "line",
			"x": -1065.9980472653137,
			"y": -104.90645869153597,
			"width": 28.238576707261018,
			"height": 27.51450179914673,
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
				"type": 2
			},
			"seed": 1983472761,
			"version": 73,
			"versionNonce": 634704729,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1693189565310,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					28.238576707261018,
					27.51450179914673
				]
			],
			"lastCommittedPoint": null,
			"startBinding": null,
			"endBinding": null,
			"startArrowhead": null,
			"endArrowhead": null
		},
		{
			"id": "6-CffG-s-eQYZTX9CS3MS",
			"type": "line",
			"x": -1067.4461970815419,
			"y": -76.66788198427518,
			"width": 29.686726523489142,
			"height": 27.5145017991467,
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
				"type": 2
			},
			"seed": 1920414679,
			"version": 62,
			"versionNonce": 1830251191,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1693189565310,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					29.686726523489142,
					-27.5145017991467
				]
			],
			"lastCommittedPoint": null,
			"startBinding": null,
			"endBinding": null,
			"startArrowhead": null,
			"endArrowhead": null
		},
		{
			"id": "BJQE2zQhSpPO2YQ-lxPjj",
			"type": "arrow",
			"x": 604.246030186484,
			"y": -248.9176775788054,
			"width": 14.906005264799433,
			"height": 106.38390038843409,
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
				"type": 2
			},
			"seed": 454142521,
			"version": 1460,
			"versionNonce": 1303643225,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1693191144327,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					14.906005264799433,
					-106.38390038843409
				]
			],
			"lastCommittedPoint": null,
			"startBinding": {
				"elementId": "84aCOpn_45bN8wEFUMFKO",
				"focus": 0.491080385160602,
				"gap": 9.933538592047398
			},
			"endBinding": {
				"elementId": "AxOREl9f",
				"focus": -0.010660554918959333,
				"gap": 6.554583177005497
			},
			"startArrowhead": null,
			"endArrowhead": "arrow"
		},
		{
			"id": "AxOREl9f",
			"type": "text",
			"x": 475.11608342543434,
			"y": -386.856161144245,
			"width": 290.2796936035156,
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
			"seed": 1801035127,
			"version": 795,
			"versionNonce": 1558961017,
			"isDeleted": false,
			"boundElements": [
				{
					"id": "BJQE2zQhSpPO2YQ-lxPjj",
					"type": "arrow"
				}
			],
			"updated": 1693191144327,
			"link": null,
			"locked": false,
			"text": "setMove(position, playerPiece)",
			"rawText": "setMove(position, playerPiece)",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 18,
			"containerId": null,
			"originalText": "setMove(position, playerPiece)",
			"lineHeight": 1.25,
			"isFrameName": false
		},
		{
			"id": "ZecfQfsApKEKUH_buQu5c",
			"type": "arrow",
			"x": -1085.8547598399814,
			"y": -218.04788046437545,
			"width": 1.2684607333449094,
			"height": 126.8445404233662,
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
				"type": 2
			},
			"seed": 448776631,
			"version": 16,
			"versionNonce": 425297017,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1693191171152,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.2684607333449094,
					-126.8445404233662
				]
			],
			"lastCommittedPoint": null,
			"startBinding": {
				"elementId": "fWRNzk4Daw9cjsjJryO8C",
				"focus": -0.04160220269494666,
				"gap": 9.774748140156532
			},
			"endBinding": {
				"elementId": "HBe9LOwN",
				"focus": 0.20521820181365022,
				"gap": 8.855797636085526
			},
			"startArrowhead": null,
			"endArrowhead": "arrow"
		},
		{
			"id": "HBe9LOwN",
			"type": "text",
			"x": -1155.8729143806127,
			"y": -403.7482185238272,
			"width": 172.2798309326172,
			"height": 50,
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
			"seed": 1139930071,
			"version": 469,
			"versionNonce": 1716116375,
			"isDeleted": false,
			"boundElements": [
				{
					"id": "ZecfQfsApKEKUH_buQu5c",
					"type": "arrow"
				}
			],
			"updated": 1693191171152,
			"link": null,
			"locked": false,
			"text": "setter & getters\n",
			"rawText": "setter & getters\n",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 43,
			"containerId": null,
			"originalText": "setter & getters\n",
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
		"scrollX": 1337.0267425480333,
		"scrollY": 768.7909599276749,
		"zoom": {
			"value": 0.6569722530249987
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