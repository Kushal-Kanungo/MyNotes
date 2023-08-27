---

excalidraw-plugin: parsed
tags: [excalidraw]

---
==⚠  Switch to EXCALIDRAW VIEW in the MORE OPTIONS menu of this document. ⚠==


# Text Elements
Basic Flow ^n2S2HUwm

idle ^Zup1sOsI

hasmoney ^37HN11RY

click on add coin ^KBepIiJr

addCoin() ^BJKtk7UK

Select Item ^p8p2Voza

cancel & refund ^oohHXbko

cancel & refund ^QTO7VNaI

select product button ^Ve4ZsYA0

return extra ^po2OOT6P

selecting product ^ZBL3mYT1

dispensing ^LoWVTUEt

dispense item ^n8sa3ZBf

Inventory performinmg different Action according to 
its state so it is an exampple of State Pattern. ^NY1wNBtY

Main Components ^f0CVaGGT

- states     => idle , hasMoney, productSelection, dispensing
- ItemType   => coke, soda, chips, biscuits
- Item        => itemType & price
- ItemShelf   => item, code & soldOut(boolean)
- Inventory   => ItemShelfs
   ^bSYc1Cwv

Interface State ^NN8VWF9u

Idle State ^5qeZUI5G

Has Money State ^DcCDpeW5

Select Product State ^JJTObSB0

dispensing ^VM3K3JMu

Vending Macine
- Inventory inventory
- State state
- List<Coin> ^OtvSLuYQ

has a  ^yByRdcI2

implementing ^gIjt6DiF

implementing ^B9Au64Mt

implementing ^ejMInuWx

implementing ^lAwawB8M

Inventory
- List<ItemShelf> shelfs ^4yUI3bpb

has a ^8P0khTQg

Item Shelf
- int code
- Item item ^VAzfkTMC

has a ^n40JnyC6

Item
- int price
- ItemType type ^m41caLrX

has a ^f41skuy2

ENUM 
ItemType ^id9ENk7L

has a ^wIQrclZn

ENUM 
Coin
- PENNY(1),
 - NICKEL(5),
- DIME(10),
     - QUARTER(25);
 ^WEHUVixD

has a ^9zBlAcRg

clickOnInsertCoinButton() ^mUjT3riE

insertCoin(coin) ^HlsauImB

refundFullMoney() ^IwxuwMjd

clickOnStartProductSelectionButton() ^YvYvrFGA

chooseProduct(machine, code) ^FtuISRUg

returnExtraMoney() ^psvVdA75

refundFullMoney() ^1saQwPVe

dispenseItem(code) ^V9S8uNsh

addItem(item, code) ^HYe8n3Yl

getItem(code) ^gNyTiIzi

updateSoldOutItem(code) ^czq6Sodj

setters & getters ^hrlOW0m9

getters & setters ^6lOsR6bp

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
			"version": 281,
			"versionNonce": 106569074,
			"isDeleted": false,
			"id": "n2S2HUwm",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -348.9289259801405,
			"y": -482.73184810075975,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 307.0556640625,
			"height": 74.42353090216336,
			"seed": 1918696878,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693068583425,
			"link": null,
			"locked": false,
			"fontSize": 59.53882472173069,
			"fontFamily": 1,
			"text": "Basic Flow",
			"rawText": "Basic Flow",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Basic Flow",
			"lineHeight": 1.25,
			"baseline": 52
		},
		{
			"type": "ellipse",
			"version": 232,
			"versionNonce": 972434094,
			"isDeleted": false,
			"id": "Gi9urIGakf7S32eX1tAg8",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -589.2357025296158,
			"y": -299.69148538838033,
			"strokeColor": "#2f9e44",
			"backgroundColor": "#b2f2bb",
			"width": 204,
			"height": 113,
			"seed": 930400434,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "Zup1sOsI"
				},
				{
					"id": "Drs1s4GuWez8RerEJnnzG",
					"type": "arrow"
				}
			],
			"updated": 1693068583425,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 187,
			"versionNonce": 668573490,
			"isDeleted": false,
			"id": "Zup1sOsI",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -516.1245712614249,
			"y": -265.64301852542025,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 57.5279541015625,
			"height": 45,
			"seed": 245154990,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693068583425,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "idle",
			"rawText": "idle",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "Gi9urIGakf7S32eX1tAg8",
			"originalText": "idle",
			"lineHeight": 1.25,
			"baseline": 32
		},
		{
			"type": "arrow",
			"version": 703,
			"versionNonce": 252981038,
			"isDeleted": false,
			"id": "Drs1s4GuWez8RerEJnnzG",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -384.278281505602,
			"y": -241.5383175459271,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 476.8775604114948,
			"height": 2.930062398126438,
			"seed": 1259774062,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "KBepIiJr"
				}
			],
			"updated": 1693134355310,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "Gi9urIGakf7S32eX1tAg8",
				"gap": 1,
				"focus": 0.018062076480438623
			},
			"endBinding": {
				"elementId": "mM8-XCUQ46u7VCAlTbtfk",
				"gap": 14.52871316621929,
				"focus": -0.015088901185557052
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
					476.8775604114948,
					2.930062398126438
				]
			]
		},
		{
			"type": "text",
			"version": 58,
			"versionNonce": 2038622450,
			"isDeleted": false,
			"id": "KBepIiJr",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -221.54067945379882,
			"y": -282.6646929640725,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 289.47589111328125,
			"height": 45,
			"seed": 1858265390,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693068583425,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "click on add coin",
			"rawText": "click on add coin",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "Drs1s4GuWez8RerEJnnzG",
			"originalText": "click on add coin",
			"lineHeight": 1.25,
			"baseline": 32
		},
		{
			"type": "ellipse",
			"version": 369,
			"versionNonce": 53597998,
			"isDeleted": false,
			"id": "mM8-XCUQ46u7VCAlTbtfk",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 107.1279397870378,
			"y": -309.17656344233603,
			"strokeColor": "#e03131",
			"backgroundColor": "#ffc9c9",
			"width": 295,
			"height": 141,
			"seed": 824001330,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "37HN11RY"
				},
				{
					"id": "Drs1s4GuWez8RerEJnnzG",
					"type": "arrow"
				},
				{
					"id": "kavXtmm0z_JrF-jJnrYpT",
					"type": "arrow"
				},
				{
					"id": "CSXKA0Bo7P-bEswyQIFch",
					"type": "arrow"
				},
				{
					"id": "C9lzQxVeqLhoYXkuhbBay",
					"type": "arrow"
				}
			],
			"updated": 1693068583425,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 378,
			"versionNonce": 1658649266,
			"isDeleted": false,
			"id": "37HN11RY",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 176.0977178212994,
			"y": -261.02759151598764,
			"strokeColor": "#e03131",
			"backgroundColor": "transparent",
			"width": 157.4639434814453,
			"height": 45,
			"seed": 1655835890,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693068583425,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "hasmoney",
			"rawText": "hasmoney",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "mM8-XCUQ46u7VCAlTbtfk",
			"originalText": "hasmoney",
			"lineHeight": 1.25,
			"baseline": 32
		},
		{
			"type": "arrow",
			"version": 222,
			"versionNonce": 1065625646,
			"isDeleted": false,
			"id": "kavXtmm0z_JrF-jJnrYpT",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 255.67314849335932,
			"y": -324.503641275497,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 5.262471600445707,
			"height": 116.96756984458636,
			"seed": 1092390706,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1693134355312,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "mM8-XCUQ46u7VCAlTbtfk",
				"gap": 15.328846113420937,
				"focus": 0.03325768604552444
			},
			"endBinding": {
				"elementId": "4O4KigLIai9nt_oLqQSBk",
				"gap": 5.172398008149239,
				"focus": 0.11365325807001493
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
					-5.262471600445707,
					-116.96756984458636
				]
			]
		},
		{
			"type": "rectangle",
			"version": 138,
			"versionNonce": 1116656754,
			"isDeleted": false,
			"id": "4O4KigLIai9nt_oLqQSBk",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 153.40028515565734,
			"y": -521.6436091282326,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 215,
			"height": 75,
			"seed": 1531534830,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "kavXtmm0z_JrF-jJnrYpT",
					"type": "arrow"
				},
				{
					"type": "text",
					"id": "BJKtk7UK"
				}
			],
			"updated": 1693068583425,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 86,
			"versionNonce": 298607534,
			"isDeleted": false,
			"id": "BJKtk7UK",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 180.9443143914972,
			"y": -506.6436091282326,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 159.9119415283203,
			"height": 45,
			"seed": 843135022,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693068583425,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "addCoin()",
			"rawText": "addCoin()",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "4O4KigLIai9nt_oLqQSBk",
			"originalText": "addCoin()",
			"lineHeight": 1.25,
			"baseline": 32
		},
		{
			"type": "arrow",
			"version": 370,
			"versionNonce": 23786094,
			"isDeleted": false,
			"id": "CSXKA0Bo7P-bEswyQIFch",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 412.1406159100303,
			"y": -249.22025491096232,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 545.855741424627,
			"height": 5.451757247576012,
			"seed": 502158066,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "Ve4ZsYA0"
				}
			],
			"updated": 1693134355312,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "mM8-XCUQ46u7VCAlTbtfk",
				"gap": 11.336485006910701,
				"focus": -0.12721374706373703
			},
			"endBinding": {
				"elementId": "z1DQHqikynGj7og7F9KLZ",
				"gap": 3.2263370675705163,
				"focus": -0.014833011847116474
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
					545.855741424627,
					-5.451757247576012
				]
			]
		},
		{
			"type": "text",
			"version": 39,
			"versionNonce": 1713356270,
			"isDeleted": false,
			"id": "Ve4ZsYA0",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 468.3196286257403,
			"y": -292.2425256847691,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 391.4998779296875,
			"height": 45,
			"seed": 320335854,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693068583426,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "select product button",
			"rawText": "select product button",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "CSXKA0Bo7P-bEswyQIFch",
			"originalText": "select product button",
			"lineHeight": 1.25,
			"baseline": 32
		},
		{
			"type": "ellipse",
			"version": 244,
			"versionNonce": 1530257394,
			"isDeleted": false,
			"id": "z1DQHqikynGj7og7F9KLZ",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 961.0688560472668,
			"y": -343.553700024342,
			"strokeColor": "#1971c2",
			"backgroundColor": "#a5d8ff",
			"width": 417,
			"height": 171,
			"seed": 2069138098,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"id": "CSXKA0Bo7P-bEswyQIFch",
					"type": "arrow"
				},
				{
					"type": "text",
					"id": "p8p2Voza"
				},
				{
					"id": "FSJNQGCNYY0gm1ph0bZPj",
					"type": "arrow"
				},
				{
					"id": "pvx_P4EUCvQ9QbLgKsXbD",
					"type": "arrow"
				},
				{
					"id": "DSr6Xczw1Joj8irW2DRLO",
					"type": "arrow"
				}
			],
			"updated": 1693068583426,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 214,
			"versionNonce": 59625518,
			"isDeleted": false,
			"id": "p8p2Voza",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1064.8411326972152,
			"y": -280.5113298157918,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 209.5919189453125,
			"height": 45,
			"seed": 565709806,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693068583426,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "Select Item",
			"rawText": "Select Item",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "z1DQHqikynGj7og7F9KLZ",
			"originalText": "Select Item",
			"lineHeight": 1.25,
			"baseline": 32
		},
		{
			"type": "arrow",
			"version": 145,
			"versionNonce": 801065838,
			"isDeleted": false,
			"id": "C9lzQxVeqLhoYXkuhbBay",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 262.6520137651589,
			"y": -157.95957297602632,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 4.204732596571603,
			"height": 128.50520050344556,
			"seed": 1019993390,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1693134355314,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "mM8-XCUQ46u7VCAlTbtfk",
				"gap": 10.321519119807288,
				"focus": -0.036490367573937484
			},
			"endBinding": {
				"elementId": "bpRAJPfzsmh0f4q9eVjuD",
				"gap": 8.05553588867197,
				"focus": 0.03498821451713924
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
					4.204732596571603,
					128.50520050344556
				]
			]
		},
		{
			"type": "rectangle",
			"version": 155,
			"versionNonce": 1711250030,
			"isDeleted": false,
			"id": "bpRAJPfzsmh0f4q9eVjuD",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 98.69614411724848,
			"y": -21.398836583908803,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#e8590c",
			"width": 329,
			"height": 116,
			"seed": 52716910,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "C9lzQxVeqLhoYXkuhbBay",
					"type": "arrow"
				},
				{
					"type": "text",
					"id": "oohHXbko"
				}
			],
			"updated": 1693068583426,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 54,
			"versionNonce": 791677810,
			"isDeleted": false,
			"id": "oohHXbko",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 123.98419953717035,
			"y": 14.101163416091197,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 278.42388916015625,
			"height": 45,
			"seed": 206330162,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693068583426,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "cancel & refund",
			"rawText": "cancel & refund",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "bpRAJPfzsmh0f4q9eVjuD",
			"originalText": "cancel & refund",
			"lineHeight": 1.25,
			"baseline": 32
		},
		{
			"type": "rectangle",
			"version": 335,
			"versionNonce": 608050350,
			"isDeleted": false,
			"id": "NS77v9MZh1E7ot2g_L1gf",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 743.1249158894834,
			"y": -41.05426854303414,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#e8590c",
			"width": 329,
			"height": 116,
			"seed": 1271064046,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "QTO7VNaI"
				},
				{
					"id": "FSJNQGCNYY0gm1ph0bZPj",
					"type": "arrow"
				}
			],
			"updated": 1693068583426,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 236,
			"versionNonce": 1539427634,
			"isDeleted": false,
			"id": "QTO7VNaI",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 768.4129713094053,
			"y": -5.554268543034141,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 278.42388916015625,
			"height": 45,
			"seed": 445380654,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693068583426,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "cancel & refund",
			"rawText": "cancel & refund",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "NS77v9MZh1E7ot2g_L1gf",
			"originalText": "cancel & refund",
			"lineHeight": 1.25,
			"baseline": 32
		},
		{
			"type": "arrow",
			"version": 371,
			"versionNonce": 1558162862,
			"isDeleted": false,
			"id": "FSJNQGCNYY0gm1ph0bZPj",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1083.0694055808503,
			"y": -167.75956483210945,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 98.67310416686053,
			"height": 105.90428685204841,
			"seed": 999298546,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1693134355314,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "z1DQHqikynGj7og7F9KLZ",
				"gap": 12.613192793130992,
				"focus": 0.010621102339126196
			},
			"endBinding": {
				"elementId": "NS77v9MZh1E7ot2g_L1gf",
				"gap": 20.80100943702689,
				"focus": 0.015333308639305522
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
					-98.67310416686053,
					105.90428685204841
				]
			]
		},
		{
			"type": "rectangle",
			"version": 76,
			"versionNonce": 473257714,
			"isDeleted": false,
			"id": "eUA3XODQlq1ghlrIGLJpn",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1240.1502420073243,
			"y": -45.67314910410994,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#e03131",
			"width": 362,
			"height": 126,
			"seed": 713473262,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "pvx_P4EUCvQ9QbLgKsXbD",
					"type": "arrow"
				},
				{
					"type": "text",
					"id": "po2OOT6P"
				}
			],
			"updated": 1693068583426,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 28,
			"versionNonce": 1839548718,
			"isDeleted": false,
			"id": "po2OOT6P",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1308.146274722168,
			"y": -5.173149104109939,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 226.0079345703125,
			"height": 45,
			"seed": 1806623986,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693068583426,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "return extra",
			"rawText": "return extra",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "eUA3XODQlq1ghlrIGLJpn",
			"originalText": "return extra",
			"lineHeight": 1.25,
			"baseline": 32
		},
		{
			"type": "arrow",
			"version": 101,
			"versionNonce": 1144637422,
			"isDeleted": false,
			"id": "pvx_P4EUCvQ9QbLgKsXbD",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1272.4637751991477,
			"y": -167.75835305372527,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 130.79615286235094,
			"height": 105.93139723387017,
			"seed": 1673630194,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1693134355315,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "z1DQHqikynGj7og7F9KLZ",
				"gap": 16.084291199573304,
				"focus": 0.03677750238839283
			},
			"endBinding": {
				"elementId": "eUA3XODQlq1ghlrIGLJpn",
				"gap": 16.15380671574516,
				"focus": 0.30852657412603757
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
					130.79615286235094,
					105.93139723387017
				]
			]
		},
		{
			"type": "arrow",
			"version": 170,
			"versionNonce": 1708562990,
			"isDeleted": false,
			"id": "DSr6Xczw1Joj8irW2DRLO",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1397.9765199795258,
			"y": -269.66636340223704,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 435.1040048415564,
			"height": 1.661280728968336,
			"seed": 857875634,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "ZBL3mYT1"
				}
			],
			"updated": 1693134355315,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "z1DQHqikynGj7og7F9KLZ",
				"gap": 21.2707211894246,
				"focus": -0.1460141621808678
			},
			"endBinding": {
				"elementId": "-apxjGmuIeii-gRf63vqU",
				"gap": 16.302967992270574,
				"focus": -0.04672886320924705
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
					435.1040048415564,
					1.661280728968336
				]
			]
		},
		{
			"type": "text",
			"version": 55,
			"versionNonce": 1912455794,
			"isDeleted": false,
			"id": "ZBL3mYT1",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1448.8245379304806,
			"y": -286.6051868446746,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 300.05987548828125,
			"height": 45,
			"seed": 497418546,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693068583426,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "selecting product",
			"rawText": "selecting product",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "DSr6Xczw1Joj8irW2DRLO",
			"originalText": "selecting product",
			"lineHeight": 1.25,
			"baseline": 32
		},
		{
			"type": "ellipse",
			"version": 79,
			"versionNonce": 126571950,
			"isDeleted": false,
			"id": "-apxjGmuIeii-gRf63vqU",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1849.2861113689655,
			"y": -357.84201243909223,
			"strokeColor": "#f08c00",
			"backgroundColor": "#ffec99",
			"width": 337,
			"height": 173,
			"seed": 909319282,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"id": "DSr6Xczw1Joj8irW2DRLO",
					"type": "arrow"
				},
				{
					"type": "text",
					"id": "LoWVTUEt"
				},
				{
					"id": "MJtcwa7Q2ybUShdxFoaHc",
					"type": "arrow"
				}
			],
			"updated": 1693068583426,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 30,
			"versionNonce": 163619890,
			"isDeleted": false,
			"id": "LoWVTUEt",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1935.4146654919618,
			"y": -294.0067490117286,
			"strokeColor": "#f08c00",
			"backgroundColor": "transparent",
			"width": 164.44790649414062,
			"height": 45,
			"seed": 1281278318,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693068583426,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "dispensing",
			"rawText": "dispensing",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "-apxjGmuIeii-gRf63vqU",
			"originalText": "dispensing",
			"lineHeight": 1.25,
			"baseline": 32
		},
		{
			"type": "rectangle",
			"version": 121,
			"versionNonce": 1798336494,
			"isDeleted": false,
			"id": "CjzNbfBBX9BeIjLH9J_tE",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1849.1693988887873,
			"y": -43.099977034844756,
			"strokeColor": "#1971c2",
			"backgroundColor": "#228be6",
			"width": 362,
			"height": 126,
			"seed": 2131509806,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "n8sa3ZBf"
				},
				{
					"id": "MJtcwa7Q2ybUShdxFoaHc",
					"type": "arrow"
				}
			],
			"updated": 1693068583426,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 85,
			"versionNonce": 1916882418,
			"isDeleted": false,
			"id": "n8sa3ZBf",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1915.1134601680842,
			"y": -2.5999770348447555,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 230.11187744140625,
			"height": 45,
			"seed": 215993454,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693068583426,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "dispense item",
			"rawText": "dispense item",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "CjzNbfBBX9BeIjLH9J_tE",
			"originalText": "dispense item",
			"lineHeight": 1.25,
			"baseline": 32
		},
		{
			"type": "arrow",
			"version": 93,
			"versionNonce": 1851549358,
			"isDeleted": false,
			"id": "MJtcwa7Q2ybUShdxFoaHc",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2023.4147405655808,
			"y": -177.26420950540634,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 6.432864580955538,
			"height": 110.96555946142857,
			"seed": 1525318066,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1693134355316,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "-apxjGmuIeii-gRf63vqU",
				"gap": 7.625881212288107,
				"focus": -0.0010367928787025844
			},
			"endBinding": {
				"elementId": "CjzNbfBBX9BeIjLH9J_tE",
				"gap": 23.198673009133017,
				"focus": 0.02531944547946245
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
					6.432864580955538,
					110.96555946142857
				]
			]
		},
		{
			"type": "text",
			"version": 283,
			"versionNonce": 1619443634,
			"isDeleted": false,
			"id": "NY1wNBtY",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -624.0726420670246,
			"y": 239.74173150785617,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 1379.6719970703125,
			"height": 133.86538066693396,
			"seed": 1019789298,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693068583426,
			"link": null,
			"locked": false,
			"fontSize": 53.54615226677358,
			"fontFamily": 1,
			"text": "Inventory performinmg different Action according to \nits state so it is an exampple of State Pattern.",
			"rawText": "Inventory performinmg different Action according to \nits state so it is an exampple of State Pattern.",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Inventory performinmg different Action according to \nits state so it is an exampple of State Pattern.",
			"lineHeight": 1.25,
			"baseline": 114
		},
		{
			"type": "text",
			"version": 82,
			"versionNonce": 1611385966,
			"isDeleted": false,
			"id": "f0CVaGGT",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -634.1254107828152,
			"y": 547.9349856895869,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#228be6",
			"width": 673.159423828125,
			"height": 104.0647690693943,
			"seed": 1013010734,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693068583426,
			"link": null,
			"locked": false,
			"fontSize": 83.25181525551544,
			"fontFamily": 1,
			"text": "Main Components",
			"rawText": "Main Components",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Main Components",
			"lineHeight": 1.25,
			"baseline": 73
		},
		{
			"type": "text",
			"version": 401,
			"versionNonce": 13920174,
			"isDeleted": false,
			"id": "bSYc1Cwv",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -653.9852571440406,
			"y": 668.2911833066827,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#228be6",
			"width": 1292.966796875,
			"height": 325.0000000000003,
			"seed": 2010051950,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693134406079,
			"link": null,
			"locked": false,
			"fontSize": 43.33333333333337,
			"fontFamily": 1,
			"text": "- states     => idle , hasMoney, productSelection, dispensing\n- ItemType   => coke, soda, chips, biscuits\n- Item        => itemType & price\n- ItemShelf   => item, code & soldOut(boolean)\n- Inventory   => ItemShelfs\n  ",
			"rawText": "- states     => idle , hasMoney, productSelection, dispensing\n- ItemType   => coke, soda, chips, biscuits\n- Item        => itemType & price\n- ItemShelf   => item, code & soldOut(boolean)\n- Inventory   => ItemShelfs\n  ",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "- states     => idle , hasMoney, productSelection, dispensing\n- ItemType   => coke, soda, chips, biscuits\n- Item        => itemType & price\n- ItemShelf   => item, code & soldOut(boolean)\n- Inventory   => ItemShelfs\n  ",
			"lineHeight": 1.25,
			"baseline": 309
		},
		{
			"type": "rectangle",
			"version": 577,
			"versionNonce": 838078126,
			"isDeleted": false,
			"id": "I24EooINj4XAn7LedaRrr",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -861.7573932348687,
			"y": 1809.9740537071361,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffec99",
			"width": 559,
			"height": 206,
			"seed": 857333806,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "NN8VWF9u"
				},
				{
					"id": "A2B0CIY1V45ndDT7I8xu_",
					"type": "arrow"
				},
				{
					"id": "aW6FvJrnc50JMQfWvg0RK",
					"type": "arrow"
				},
				{
					"id": "gK9sCSAoWd-goJ-wpbtOw",
					"type": "arrow"
				},
				{
					"id": "biH5VIujVWLsytnT8k2ap",
					"type": "arrow"
				},
				{
					"id": "8KGTC4eb9j8252QresTuU",
					"type": "arrow"
				}
			],
			"updated": 1693068583426,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 447,
			"versionNonce": 572259122,
			"isDeleted": false,
			"id": "NN8VWF9u",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -730.0013507543999,
			"y": 1890.4740537071361,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffec99",
			"width": 295.4879150390625,
			"height": 45,
			"seed": 438748526,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693068583426,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "Interface State",
			"rawText": "Interface State",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "I24EooINj4XAn7LedaRrr",
			"originalText": "Interface State",
			"lineHeight": 1.25,
			"baseline": 32
		},
		{
			"type": "rectangle",
			"version": 507,
			"versionNonce": 437913838,
			"isDeleted": false,
			"id": "UCab9n1wCyc7eI2GZw1xB",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1531.949639180656,
			"y": 2184.880117827342,
			"strokeColor": "#1971c2",
			"backgroundColor": "#a5d8ff",
			"width": 399,
			"height": 189,
			"seed": 227595442,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "5qeZUI5G"
				},
				{
					"id": "aW6FvJrnc50JMQfWvg0RK",
					"type": "arrow"
				},
				{
					"id": "E-ON-jYU6V-DelvnyIR1K",
					"type": "arrow"
				}
			],
			"updated": 1693068583426,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 413,
			"versionNonce": 857326834,
			"isDeleted": false,
			"id": "5qeZUI5G",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1429.2176064047771,
			"y": 2256.880117827342,
			"strokeColor": "#1971c2",
			"backgroundColor": "#a5d8ff",
			"width": 193.5359344482422,
			"height": 45,
			"seed": 927199346,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693068583426,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "Idle State",
			"rawText": "Idle State",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "UCab9n1wCyc7eI2GZw1xB",
			"originalText": "Idle State",
			"lineHeight": 1.25,
			"baseline": 32
		},
		{
			"type": "rectangle",
			"version": 648,
			"versionNonce": 1547133938,
			"isDeleted": false,
			"id": "Gxs1Msljc-v-ybp0c6i01",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1042.4485603943008,
			"y": 2187.5637807640196,
			"strokeColor": "#1971c2",
			"backgroundColor": "#a5d8ff",
			"width": 399,
			"height": 189,
			"seed": 995006322,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "DcCDpeW5"
				},
				{
					"id": "A2B0CIY1V45ndDT7I8xu_",
					"type": "arrow"
				},
				{
					"id": "URxYe1rBrqDzPQvXVRxzq",
					"type": "arrow"
				},
				{
					"id": "nhWqa63qOZsQ53CvTNbX_",
					"type": "arrow"
				},
				{
					"id": "12iWnj8UEvYGc4ZaoT8ff",
					"type": "arrow"
				}
			],
			"updated": 1693068664658,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 582,
			"versionNonce": 2100844210,
			"isDeleted": false,
			"id": "DcCDpeW5",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -996.2365242614883,
			"y": 2259.5637807640196,
			"strokeColor": "#1971c2",
			"backgroundColor": "#a5d8ff",
			"width": 306.575927734375,
			"height": 45,
			"seed": 2083445042,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693068583426,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "Has Money State",
			"rawText": "Has Money State",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "Gxs1Msljc-v-ybp0c6i01",
			"originalText": "Has Money State",
			"lineHeight": 1.25,
			"baseline": 32
		},
		{
			"type": "rectangle",
			"version": 801,
			"versionNonce": 1539830642,
			"isDeleted": false,
			"id": "tkwgFcuUz980ocUx-W7OL",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -573.0277440854189,
			"y": 2189.806340378412,
			"strokeColor": "#1971c2",
			"backgroundColor": "#a5d8ff",
			"width": 440,
			"height": 189,
			"seed": 1781915822,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "JJTObSB0"
				},
				{
					"id": "gK9sCSAoWd-goJ-wpbtOw",
					"type": "arrow"
				},
				{
					"id": "L-a2MYhX0S8W76iXxMMCA",
					"type": "arrow"
				},
				{
					"id": "B9Sz2clwfKd_xXkdMxGVL",
					"type": "arrow"
				},
				{
					"id": "4lKBbfZ6mz6K5xwUKM3C1",
					"type": "arrow"
				}
			],
			"updated": 1693068879947,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 779,
			"versionNonce": 824094834,
			"isDeleted": false,
			"id": "JJTObSB0",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -548.0216863461611,
			"y": 2261.806340378412,
			"strokeColor": "#1971c2",
			"backgroundColor": "#a5d8ff",
			"width": 389.9878845214844,
			"height": 45,
			"seed": 1313970926,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693068583426,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "Select Product State",
			"rawText": "Select Product State",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "tkwgFcuUz980ocUx-W7OL",
			"originalText": "Select Product State",
			"lineHeight": 1.25,
			"baseline": 32
		},
		{
			"type": "arrow",
			"version": 1312,
			"versionNonce": 564680878,
			"isDeleted": false,
			"id": "A2B0CIY1V45ndDT7I8xu_",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -773.5440982073771,
			"y": 2170.5969007688686,
			"strokeColor": "#1971c2",
			"backgroundColor": "#a5d8ff",
			"width": 93.24122808418906,
			"height": 140.18029367274903,
			"seed": 664085298,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "ejMInuWx"
				}
			],
			"updated": 1693134355323,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "Gxs1Msljc-v-ybp0c6i01",
				"gap": 16.966879995150975,
				"focus": -0.018059279187015068
			},
			"endBinding": {
				"elementId": "I24EooINj4XAn7LedaRrr",
				"gap": 14.44255338898347,
				"focus": 0.0572634916071992
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "triangle",
			"points": [
				[
					0,
					0
				],
				[
					93.24122808418906,
					-140.18029367274903
				]
			]
		},
		{
			"type": "text",
			"version": 51,
			"versionNonce": 1385419314,
			"isDeleted": false,
			"id": "ejMInuWx",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -821.1273088453504,
			"y": 2072.310472508051,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#3bc9db",
			"width": 199.9438934326172,
			"height": 45,
			"seed": 2113957426,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693068583426,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "implementing",
			"rawText": "implementing",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "A2B0CIY1V45ndDT7I8xu_",
			"originalText": "implementing",
			"lineHeight": 1.25,
			"baseline": 32
		},
		{
			"type": "arrow",
			"version": 1182,
			"versionNonce": 488049710,
			"isDeleted": false,
			"id": "aW6FvJrnc50JMQfWvg0RK",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1175.9952830304235,
			"y": 2173.7162884802733,
			"strokeColor": "#1971c2",
			"backgroundColor": "#a5d8ff",
			"width": 318.8355605297703,
			"height": 146.71255859603025,
			"seed": 1826569266,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "lAwawB8M"
				}
			],
			"updated": 1693134355322,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "UCab9n1wCyc7eI2GZw1xB",
				"gap": 11.163829347068713,
				"focus": -0.18073751275855685
			},
			"endBinding": {
				"elementId": "I24EooINj4XAn7LedaRrr",
				"gap": 11.029676177106921,
				"focus": 0.053826833866034915
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "triangle",
			"points": [
				[
					0,
					0
				],
				[
					318.8355605297703,
					-146.71255859603025
				]
			]
		},
		{
			"type": "text",
			"version": 51,
			"versionNonce": 1417591794,
			"isDeleted": false,
			"id": "lAwawB8M",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1117.1193085911686,
			"y": 2078.785946410991,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#3bc9db",
			"width": 199.9438934326172,
			"height": 45,
			"seed": 307308082,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693068583426,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "implementing",
			"rawText": "implementing",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "aW6FvJrnc50JMQfWvg0RK",
			"originalText": "implementing",
			"lineHeight": 1.25,
			"baseline": 32
		},
		{
			"type": "arrow",
			"version": 1335,
			"versionNonce": 267882926,
			"isDeleted": false,
			"id": "gK9sCSAoWd-goJ-wpbtOw",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -452.78791682235124,
			"y": 2161.5062417220397,
			"strokeColor": "#1971c2",
			"backgroundColor": "#a5d8ff",
			"width": 50.67099168683637,
			"height": 129.57452010177258,
			"seed": 834231154,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "B9Au64Mt"
				}
			],
			"updated": 1693134355325,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "tkwgFcuUz980ocUx-W7OL",
				"gap": 28.300098656372484,
				"focus": -0.20135195579784815
			},
			"endBinding": {
				"elementId": "I24EooINj4XAn7LedaRrr",
				"gap": 15.95766791313099,
				"focus": -0.1009425270998774
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "triangle",
			"points": [
				[
					0,
					0
				],
				[
					-50.67099168683637,
					-129.57452010177258
				]
			]
		},
		{
			"type": "text",
			"version": 55,
			"versionNonce": 887516594,
			"isDeleted": false,
			"id": "B9Au64Mt",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -589.1950487943823,
			"y": 2068.522630711176,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#3bc9db",
			"width": 199.9438934326172,
			"height": 45,
			"seed": 2141354798,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693068583426,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "implementing",
			"rawText": "implementing",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "gK9sCSAoWd-goJ-wpbtOw",
			"originalText": "implementing",
			"lineHeight": 1.25,
			"baseline": 32
		},
		{
			"type": "rectangle",
			"version": 822,
			"versionNonce": 183456114,
			"isDeleted": false,
			"id": "5EF41dO5cDptKyn1NAywq",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -92.12130361834693,
			"y": 2186.9257639250263,
			"strokeColor": "#1971c2",
			"backgroundColor": "#a5d8ff",
			"width": 440,
			"height": 189,
			"seed": 2080735986,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "VM3K3JMu"
				},
				{
					"id": "biH5VIujVWLsytnT8k2ap",
					"type": "arrow"
				},
				{
					"id": "E4UHnZMt_6FO-tpKu63ID",
					"type": "arrow"
				}
			],
			"updated": 1693069038770,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 811,
			"versionNonce": 418506610,
			"isDeleted": false,
			"id": "VM3K3JMu",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 45.65474313458276,
			"y": 2258.9257639250263,
			"strokeColor": "#1971c2",
			"backgroundColor": "#a5d8ff",
			"width": 164.44790649414062,
			"height": 45,
			"seed": 1845253298,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693068583426,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "dispensing",
			"rawText": "dispensing",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "5EF41dO5cDptKyn1NAywq",
			"originalText": "dispensing",
			"lineHeight": 1.25,
			"baseline": 32
		},
		{
			"type": "arrow",
			"version": 1190,
			"versionNonce": 878856878,
			"isDeleted": false,
			"id": "biH5VIujVWLsytnT8k2ap",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 34.066741086072426,
			"y": 2172.0317875400833,
			"strokeColor": "#1971c2",
			"backgroundColor": "#a5d8ff",
			"width": 372.04209653507576,
			"height": 141.61518044396416,
			"seed": 1697876466,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "gIjt6DiF"
				}
			],
			"updated": 1693134355326,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "5EF41dO5cDptKyn1NAywq",
				"gap": 14.893976384943016,
				"focus": 0.41340062971803354
			},
			"endBinding": {
				"elementId": "I24EooINj4XAn7LedaRrr",
				"gap": 14.442553388983015,
				"focus": 0.11680771679616121
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "triangle",
			"points": [
				[
					0,
					0
				],
				[
					-372.04209653507576,
					-141.61518044396416
				]
			]
		},
		{
			"type": "text",
			"version": 86,
			"versionNonce": 1760045362,
			"isDeleted": false,
			"id": "gIjt6DiF",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -251.56281063311894,
			"y": 2073.9772150062754,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#3bc9db",
			"width": 199.9438934326172,
			"height": 45,
			"seed": 550483506,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693068583426,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "implementing",
			"rawText": "implementing",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "biH5VIujVWLsytnT8k2ap",
			"originalText": "implementing",
			"lineHeight": 1.25,
			"baseline": 32
		},
		{
			"type": "rectangle",
			"version": 850,
			"versionNonce": 1494148462,
			"isDeleted": false,
			"id": "9ELL9gTEMvRnyhxrGJE4V",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 431.0568612964307,
			"y": 1759.2270562884169,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#3bc9db",
			"width": 636,
			"height": 265,
			"seed": 1820882798,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "OtvSLuYQ"
				},
				{
					"id": "8KGTC4eb9j8252QresTuU",
					"type": "arrow"
				},
				{
					"id": "NIfxMsNpAldzGW6C4V9KT",
					"type": "arrow"
				},
				{
					"id": "h2xL2SJFQptymMSKIwYhv",
					"type": "arrow"
				},
				{
					"id": "dAUjC9lDjF-Yv4TLkA_Va",
					"type": "arrow"
				}
			],
			"updated": 1693109676076,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 864,
			"versionNonce": 1815098098,
			"isDeleted": false,
			"id": "OtvSLuYQ",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 565.1149362476026,
			"y": 1801.7270562884169,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#a5d8ff",
			"width": 367.88385009765625,
			"height": 180,
			"seed": 138330418,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693068583426,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "Vending Macine\n- Inventory inventory\n- State state\n- List<Coin>",
			"rawText": "Vending Macine\n- Inventory inventory\n- State state\n- List<Coin>",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "9ELL9gTEMvRnyhxrGJE4V",
			"originalText": "Vending Macine\n- Inventory inventory\n- State state\n- List<Coin>",
			"lineHeight": 1.25,
			"baseline": 167
		},
		{
			"type": "arrow",
			"version": 821,
			"versionNonce": 689305390,
			"isDeleted": false,
			"id": "8KGTC4eb9j8252QresTuU",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 419.57768591163494,
			"y": 1881.8913989816892,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#3bc9db",
			"width": 709.1021741510119,
			"height": 2.5632799146512752,
			"seed": 1517748018,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "yByRdcI2"
				}
			],
			"updated": 1693134355327,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "9ELL9gTEMvRnyhxrGJE4V",
				"gap": 11.47917538479578,
				"focus": 0.08250435304803656
			},
			"endBinding": {
				"elementId": "I24EooINj4XAn7LedaRrr",
				"gap": 13.232904995491708,
				"focus": -0.2640237097798915
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "triangle",
			"points": [
				[
					0,
					0
				],
				[
					-709.1021741510119,
					2.5632799146512752
				]
			]
		},
		{
			"type": "text",
			"version": 56,
			"versionNonce": 1699808434,
			"isDeleted": false,
			"id": "yByRdcI2",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 101.70809305343016,
			"y": 1866.2236247381566,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#3bc9db",
			"width": 121.35597229003906,
			"height": 45,
			"seed": 238814894,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693068583426,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "has a ",
			"rawText": "has a ",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "8KGTC4eb9j8252QresTuU",
			"originalText": "has a ",
			"lineHeight": 1.25,
			"baseline": 32
		},
		{
			"type": "rectangle",
			"version": 1050,
			"versionNonce": 1589299886,
			"isDeleted": false,
			"id": "4VkNprePekffGKV4CuHrh",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1500.5568930801996,
			"y": 1763.1630820480327,
			"strokeColor": "#2f9e44",
			"backgroundColor": "#b2f2bb",
			"width": 636,
			"height": 265,
			"seed": 1449444974,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "4yUI3bpb"
				},
				{
					"id": "NIfxMsNpAldzGW6C4V9KT",
					"type": "arrow"
				},
				{
					"id": "79Kki8R2PHu-RP45hAZPs",
					"type": "arrow"
				},
				{
					"id": "pqx70_1R50jFEHbxsqwxK",
					"type": "arrow"
				},
				{
					"id": "shoP5RhvssGVDhi7LHhrl",
					"type": "arrow"
				},
				{
					"id": "bfcv3TKmRBE591D2Rr3kH",
					"type": "arrow"
				}
			],
			"updated": 1693109514647,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 1043,
			"versionNonce": 770809458,
			"isDeleted": false,
			"id": "4yUI3bpb",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1602.7189719376215,
			"y": 1850.6630820480327,
			"strokeColor": "#2f9e44",
			"backgroundColor": "#a5d8ff",
			"width": 431.67584228515625,
			"height": 90,
			"seed": 656263342,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693068583426,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "Inventory\n- List<ItemShelf> shelfs",
			"rawText": "Inventory\n- List<ItemShelf> shelfs",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "4VkNprePekffGKV4CuHrh",
			"originalText": "Inventory\n- List<ItemShelf> shelfs",
			"lineHeight": 1.25,
			"baseline": 77
		},
		{
			"type": "arrow",
			"version": 1146,
			"versionNonce": 107081774,
			"isDeleted": false,
			"id": "NIfxMsNpAldzGW6C4V9KT",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1075.822314341388,
			"y": 1881.3153971017812,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#b2f2bb",
			"width": 400.7242073818411,
			"height": 4.028261089602665,
			"seed": 1522850610,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "8P0khTQg"
				}
			],
			"updated": 1693134355329,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "9ELL9gTEMvRnyhxrGJE4V",
				"gap": 8.765453044957212,
				"focus": -0.10093433139131472
			},
			"endBinding": {
				"elementId": "4VkNprePekffGKV4CuHrh",
				"gap": 24.01037135697061,
				"focus": 0.050711489943730884
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "triangle",
			"points": [
				[
					0,
					0
				],
				[
					400.7242073818411,
					4.028261089602665
				]
			]
		},
		{
			"type": "text",
			"version": 55,
			"versionNonce": 1389953074,
			"isDeleted": false,
			"id": "8P0khTQg",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1304.317301209704,
			"y": 1878.9776340298718,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#b2f2bb",
			"width": 103.35597229003906,
			"height": 45,
			"seed": 1725709742,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693068583426,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "has a",
			"rawText": "has a",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "NIfxMsNpAldzGW6C4V9KT",
			"originalText": "has a",
			"lineHeight": 1.25,
			"baseline": 32
		},
		{
			"type": "rectangle",
			"version": 1522,
			"versionNonce": 1644431022,
			"isDeleted": false,
			"id": "c2Ib2u-lPAJoZqhkxRaVH",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1533.2364387743164,
			"y": 2217.037149607741,
			"strokeColor": "#e03131",
			"backgroundColor": "#ffc9c9",
			"width": 636,
			"height": 265,
			"seed": 1147275762,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "VAzfkTMC"
				},
				{
					"id": "79Kki8R2PHu-RP45hAZPs",
					"type": "arrow"
				},
				{
					"id": "g25PrH1c1X_lKHJWv2ztp",
					"type": "arrow"
				},
				{
					"id": "qnWfmyXs62AV2rmp86Yom",
					"type": "arrow"
				}
			],
			"updated": 1693109605644,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 1531,
			"versionNonce": 804137458,
			"isDeleted": false,
			"id": "VAzfkTMC",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1749.266475700586,
			"y": 2282.037149607741,
			"strokeColor": "#e03131",
			"backgroundColor": "#a5d8ff",
			"width": 203.93992614746094,
			"height": 135,
			"seed": 657456050,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693068583426,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "Item Shelf\n- int code\n- Item item",
			"rawText": "Item Shelf\n- int code\n- Item item",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "c2Ib2u-lPAJoZqhkxRaVH",
			"originalText": "Item Shelf\n- int code\n- Item item",
			"lineHeight": 1.25,
			"baseline": 122
		},
		{
			"type": "arrow",
			"version": 1048,
			"versionNonce": 184554350,
			"isDeleted": false,
			"id": "79Kki8R2PHu-RP45hAZPs",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1816.7813650348376,
			"y": 2035.2962672253593,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#b2f2bb",
			"width": 0.11849420634598573,
			"height": 167.88907574175664,
			"seed": 1241407214,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "n40JnyC6"
				}
			],
			"updated": 1693134355330,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "4VkNprePekffGKV4CuHrh",
				"gap": 7.133185177326595,
				"focus": 0.005271963212715065
			},
			"endBinding": {
				"elementId": "c2Ib2u-lPAJoZqhkxRaVH",
				"gap": 13.851806640625,
				"focus": -0.1090146750524069
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "triangle",
			"points": [
				[
					0,
					0
				],
				[
					-0.11849420634598573,
					167.88907574175664
				]
			]
		},
		{
			"type": "text",
			"version": 70,
			"versionNonce": 205003698,
			"isDeleted": false,
			"id": "n40JnyC6",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2449.6511166350765,
			"y": 1918.2761544474392,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#b2f2bb",
			"width": 103.35597229003906,
			"height": 45,
			"seed": 1701985138,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693068583426,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "has a",
			"rawText": "has a",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "79Kki8R2PHu-RP45hAZPs",
			"originalText": "has a",
			"lineHeight": 1.25,
			"baseline": 32
		},
		{
			"type": "rectangle",
			"version": 1882,
			"versionNonce": 128856174,
			"isDeleted": false,
			"id": "1OVJxxbq3Dl-BJDXYzVQR",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1480.8396719943034,
			"y": 2726.818709288336,
			"strokeColor": "#9c36b5",
			"backgroundColor": "#eebefa",
			"width": 636,
			"height": 265,
			"seed": 466892594,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "m41caLrX"
				},
				{
					"id": "g25PrH1c1X_lKHJWv2ztp",
					"type": "arrow"
				},
				{
					"id": "xnyWlmxDoDi4E3Tk1AkFn",
					"type": "arrow"
				}
			],
			"updated": 1693068583426,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 1916,
			"versionNonce": 903730546,
			"isDeleted": false,
			"id": "m41caLrX",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1653.2557333956706,
			"y": 2791.818709288336,
			"strokeColor": "#9c36b5",
			"backgroundColor": "#a5d8ff",
			"width": 291.1678771972656,
			"height": 135,
			"seed": 1114276082,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693068583427,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "Item\n- int price\n- ItemType type",
			"rawText": "Item\n- int price\n- ItemType type",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "1OVJxxbq3Dl-BJDXYzVQR",
			"originalText": "Item\n- int price\n- ItemType type",
			"lineHeight": 1.25,
			"baseline": 122
		},
		{
			"type": "arrow",
			"version": 653,
			"versionNonce": 476865070,
			"isDeleted": false,
			"id": "g25PrH1c1X_lKHJWv2ztp",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1820.4849252873598,
			"y": 2499.065715470345,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#eebefa",
			"width": 3.25011089189843,
			"height": 212.79082843346214,
			"seed": 1805310190,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "f41skuy2"
				}
			],
			"updated": 1693134355331,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "c2Ib2u-lPAJoZqhkxRaVH",
				"gap": 17.028565862603955,
				"focus": 0.10322787439502717
			},
			"endBinding": {
				"elementId": "1OVJxxbq3Dl-BJDXYzVQR",
				"gap": 14.962165384528817,
				"focus": 0.08483014351915268
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "triangle",
			"points": [
				[
					0,
					0
				],
				[
					3.25011089189843,
					212.79082843346214
				]
			]
		},
		{
			"type": "text",
			"version": 20,
			"versionNonce": 505829170,
			"isDeleted": false,
			"id": "f41skuy2",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2248.240194539486,
			"y": 2317.5865199146665,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#eebefa",
			"width": 103.35597229003906,
			"height": 45,
			"seed": 590477746,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693068583427,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "has a",
			"rawText": "has a",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "g25PrH1c1X_lKHJWv2ztp",
			"originalText": "has a",
			"lineHeight": 1.25,
			"baseline": 32
		},
		{
			"type": "rectangle",
			"version": 2005,
			"versionNonce": 2138270958,
			"isDeleted": false,
			"id": "HlvRAtpiGqpRXbk7owskC",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 538.1602238315174,
			"y": 2739.923179069516,
			"strokeColor": "#1971c2",
			"backgroundColor": "#a5d8ff",
			"width": 636,
			"height": 265,
			"seed": 894402738,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "id9ENk7L"
				},
				{
					"id": "xnyWlmxDoDi4E3Tk1AkFn",
					"type": "arrow"
				}
			],
			"updated": 1693068583427,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 2062,
			"versionNonce": 1970839794,
			"isDeleted": false,
			"id": "id9ENk7L",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 773.3062580722401,
			"y": 2827.423179069516,
			"strokeColor": "#1971c2",
			"backgroundColor": "#a5d8ff",
			"width": 165.7079315185547,
			"height": 90,
			"seed": 1891670642,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693068583427,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "ENUM \nItemType",
			"rawText": "ENUM \nItemType",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "HlvRAtpiGqpRXbk7owskC",
			"originalText": "ENUM \nItemType",
			"lineHeight": 1.25,
			"baseline": 77
		},
		{
			"type": "arrow",
			"version": 145,
			"versionNonce": 1075850926,
			"isDeleted": false,
			"id": "xnyWlmxDoDi4E3Tk1AkFn",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1473.2711450554755,
			"y": 2852.3453640198604,
			"strokeColor": "#1971c2",
			"backgroundColor": "#a5d8ff",
			"width": 287.77766927083303,
			"height": 4.942347217262977,
			"seed": 319585326,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "wIQrclZn"
				}
			],
			"updated": 1693134355332,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "1OVJxxbq3Dl-BJDXYzVQR",
				"gap": 7.568526938827972,
				"focus": 0.01001720844290434
			},
			"endBinding": {
				"elementId": "HlvRAtpiGqpRXbk7owskC",
				"gap": 11.333251953125,
				"focus": -0.22235346088778934
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "triangle",
			"points": [
				[
					0,
					0
				],
				[
					-287.77766927083303,
					-4.942347217262977
				]
			]
		},
		{
			"type": "text",
			"version": 18,
			"versionNonce": 1197191858,
			"isDeleted": false,
			"id": "wIQrclZn",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1245.7598459221747,
			"y": 2823.534324089047,
			"strokeColor": "#1971c2",
			"backgroundColor": "#a5d8ff",
			"width": 103.35597229003906,
			"height": 45,
			"seed": 1904391534,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693068583427,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "has a",
			"rawText": "has a",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "xnyWlmxDoDi4E3Tk1AkFn",
			"originalText": "has a",
			"lineHeight": 1.25,
			"baseline": 32
		},
		{
			"type": "rectangle",
			"version": 2343,
			"versionNonce": 863209838,
			"isDeleted": false,
			"id": "XXuyg10AMF0DtY0x0fUr2",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 404.9564194165314,
			"y": 1053.3329758716309,
			"strokeColor": "#1971c2",
			"backgroundColor": "#a5d8ff",
			"width": 636,
			"height": 325,
			"seed": 1946501298,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "WEHUVixD"
				},
				{
					"id": "h2xL2SJFQptymMSKIwYhv",
					"type": "arrow"
				}
			],
			"updated": 1693068583427,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 2430,
			"versionNonce": 376867954,
			"isDeleted": false,
			"id": "WEHUVixD",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 531.0584701977814,
			"y": 1058.3329758716309,
			"strokeColor": "#1971c2",
			"backgroundColor": "#a5d8ff",
			"width": 383.7958984375,
			"height": 315,
			"seed": 1388206706,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693068583427,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "ENUM \nCoin\n- PENNY(1),\n - NICKEL(5),\n- DIME(10),\n     - QUARTER(25);\n",
			"rawText": "ENUM \nCoin\n- PENNY(1),\n - NICKEL(5),\n- DIME(10),\n     - QUARTER(25);\n",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "XXuyg10AMF0DtY0x0fUr2",
			"originalText": "ENUM \nCoin\n- PENNY(1),\n - NICKEL(5),\n- DIME(10),\n     - QUARTER(25);\n",
			"lineHeight": 1.25,
			"baseline": 302
		},
		{
			"type": "arrow",
			"version": 439,
			"versionNonce": 1304570094,
			"isDeleted": false,
			"id": "h2xL2SJFQptymMSKIwYhv",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 767.6522157946362,
			"y": 1746.0785548657307,
			"strokeColor": "#1971c2",
			"backgroundColor": "#a5d8ff",
			"width": 6.0404481217887,
			"height": 353.74995422363304,
			"seed": 357802034,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "9zBlAcRg"
				}
			],
			"updated": 1693134355333,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "9ELL9gTEMvRnyhxrGJE4V",
				"gap": 13.148501422686422,
				"focus": 0.05029751459193813
			},
			"endBinding": {
				"elementId": "XXuyg10AMF0DtY0x0fUr2",
				"gap": 13.995624770466748,
				"focus": -0.16756302828626815
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "triangle",
			"points": [
				[
					0,
					0
				],
				[
					6.0404481217887,
					-353.74995422363304
				]
			]
		},
		{
			"type": "text",
			"version": 18,
			"versionNonce": 2022714930,
			"isDeleted": false,
			"id": "9zBlAcRg",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 710.9556198973012,
			"y": 1618.3702342480547,
			"strokeColor": "#1971c2",
			"backgroundColor": "#a5d8ff",
			"width": 103.35597229003906,
			"height": 45,
			"seed": 2060943666,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693068583427,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "has a",
			"rawText": "has a",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "h2xL2SJFQptymMSKIwYhv",
			"originalText": "has a",
			"lineHeight": 1.25,
			"baseline": 32
		},
		{
			"type": "arrow",
			"version": 162,
			"versionNonce": 1929467502,
			"isDeleted": false,
			"id": "E-ON-jYU6V-DelvnyIR1K",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1431.9733330371848,
			"y": 2383.4343806229544,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 98.09276311083318,
			"height": 87.96296013726169,
			"seed": 175825970,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1693134355322,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "UCab9n1wCyc7eI2GZw1xB",
				"gap": 9.55426279561243,
				"focus": -0.05346030127749381
			},
			"endBinding": {
				"elementId": "mUjT3riE",
				"gap": 4.444444444444343,
				"focus": -0.2660261804896174
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
					-98.09276311083318,
					87.96296013726169
				]
			]
		},
		{
			"type": "text",
			"version": 102,
			"versionNonce": 1127399598,
			"isDeleted": false,
			"id": "mUjT3riE",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1716.5480462084222,
			"y": 2475.8417852046605,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 444.4558410644531,
			"height": 45,
			"seed": 168124206,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "E-ON-jYU6V-DelvnyIR1K",
					"type": "arrow"
				}
			],
			"updated": 1693068694324,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "clickOnInsertCoinButton()",
			"rawText": "clickOnInsertCoinButton()",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "clickOnInsertCoinButton()",
			"lineHeight": 1.25,
			"baseline": 32
		},
		{
			"type": "arrow",
			"version": 476,
			"versionNonce": 1622479598,
			"isDeleted": false,
			"id": "URxYe1rBrqDzPQvXVRxzq",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -911.8663341591443,
			"y": 2386.619613522824,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 140.0420091258618,
			"height": 109.71813188232818,
			"seed": 279451762,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1693134355324,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "Gxs1Msljc-v-ybp0c6i01",
				"gap": 10.055832758804172,
				"focus": -0.20145672418914165
			},
			"endBinding": {
				"elementId": "HlsauImB",
				"gap": 1,
				"focus": -0.043654025483502494
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
					-140.0420091258618,
					109.71813188232818
				]
			]
		},
		{
			"type": "text",
			"version": 275,
			"versionNonce": 527762994,
			"isDeleted": false,
			"id": "HlsauImB",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1203.7312690810268,
			"y": 2497.337745405152,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 257.39990234375,
			"height": 45,
			"seed": 516826098,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "URxYe1rBrqDzPQvXVRxzq",
					"type": "arrow"
				}
			],
			"updated": 1693068810269,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "insertCoin(coin)",
			"rawText": "insertCoin(coin)",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "insertCoin(coin)",
			"lineHeight": 1.25,
			"baseline": 32
		},
		{
			"type": "arrow",
			"version": 474,
			"versionNonce": 179340590,
			"isDeleted": false,
			"id": "nhWqa63qOZsQ53CvTNbX_",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -856.8143961133038,
			"y": 2387.6936850934408,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 114.18349905187847,
			"height": 213.99464634486594,
			"seed": 154629998,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1693134355324,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "Gxs1Msljc-v-ybp0c6i01",
				"gap": 11.129904329421151,
				"focus": -0.16997014203397326
			},
			"endBinding": {
				"elementId": "IwxuwMjd",
				"gap": 6.29638671875,
				"focus": 0.01957473076818956
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
					-114.18349905187847,
					213.99464634486594
				]
			]
		},
		{
			"type": "text",
			"version": 265,
			"versionNonce": 1015970738,
			"isDeleted": false,
			"id": "IwxuwMjd",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1138.7573313995497,
			"y": 2607.9847181570567,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 298.4758605957031,
			"height": 45,
			"seed": 2034674098,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "nhWqa63qOZsQ53CvTNbX_",
					"type": "arrow"
				}
			],
			"updated": 1693068687948,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "refundFullMoney()",
			"rawText": "refundFullMoney()",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "refundFullMoney()",
			"lineHeight": 1.25,
			"baseline": 32
		},
		{
			"type": "text",
			"version": 169,
			"versionNonce": 1745497202,
			"isDeleted": false,
			"id": "YvYvrFGA",
			"fillStyle": "hachure",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1270.0678969380901,
			"y": 2729.5178626215443,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 659.5557861328125,
			"height": 45,
			"seed": 1098379762,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "12iWnj8UEvYGc4ZaoT8ff",
					"type": "arrow"
				}
			],
			"updated": 1693068889878,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "clickOnStartProductSelectionButton()",
			"rawText": "clickOnStartProductSelectionButton()",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "clickOnStartProductSelectionButton()",
			"lineHeight": 1.25,
			"baseline": 32
		},
		{
			"type": "arrow",
			"version": 207,
			"versionNonce": 1090760558,
			"isDeleted": false,
			"id": "12iWnj8UEvYGc4ZaoT8ff",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -755.5257653614632,
			"y": 2387.6936647483885,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 98.5707568591755,
			"height": 338.4908238497187,
			"seed": 1956452658,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1693134355324,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "Gxs1Msljc-v-ybp0c6i01",
				"gap": 11.129883984368917,
				"focus": -0.5206047751321948
			},
			"endBinding": {
				"elementId": "YvYvrFGA",
				"gap": 3.3333740234370453,
				"focus": 0.23390902797719013
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
					-98.5707568591755,
					338.4908238497187
				]
			]
		},
		{
			"type": "arrow",
			"version": 614,
			"versionNonce": 313863150,
			"isDeleted": false,
			"id": "L-a2MYhX0S8W76iXxMMCA",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -539.5993912875056,
			"y": 2387.679203457902,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 67.4173545303588,
			"height": 209.52346467467942,
			"seed": 1925650286,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1693134355325,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "tkwgFcuUz980ocUx-W7OL",
				"gap": 8.872863079489889,
				"focus": 0.612205777987961
			},
			"endBinding": {
				"elementId": "FtuISRUg",
				"gap": 11.899393044627232,
				"focus": -0.5508403089673674
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
					-67.4173545303588,
					209.52346467467942
				]
			]
		},
		{
			"type": "text",
			"version": 318,
			"versionNonce": 290680946,
			"isDeleted": false,
			"id": "FtuISRUg",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -729.3391137037764,
			"y": 2609.1020611772087,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 513.1438598632812,
			"height": 45,
			"seed": 104276590,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "L-a2MYhX0S8W76iXxMMCA",
					"type": "arrow"
				}
			],
			"updated": 1693068853081,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "chooseProduct(machine, code)",
			"rawText": "chooseProduct(machine, code)",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "chooseProduct(machine, code)",
			"lineHeight": 1.25,
			"baseline": 32
		},
		{
			"type": "text",
			"version": 44,
			"versionNonce": 458026158,
			"isDeleted": false,
			"id": "psvVdA75",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -537.6761056962752,
			"y": 2531.148857498604,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 340.5959167480469,
			"height": 45,
			"seed": 1141194350,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "B9Sz2clwfKd_xXkdMxGVL",
					"type": "arrow"
				}
			],
			"updated": 1693068865912,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "returnExtraMoney()",
			"rawText": "returnExtraMoney()",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "returnExtraMoney()",
			"lineHeight": 1.25,
			"baseline": 32
		},
		{
			"type": "arrow",
			"version": 54,
			"versionNonce": 390430254,
			"isDeleted": false,
			"id": "B9Sz2clwfKd_xXkdMxGVL",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -467.89882507351126,
			"y": 2392.1741626549706,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 23.194656075769274,
			"height": 129.50352001787041,
			"seed": 304596466,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1693134355325,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "tkwgFcuUz980ocUx-W7OL",
				"gap": 13.3678222765584,
				"focus": 0.40329777485468643
			},
			"endBinding": {
				"elementId": "psvVdA75",
				"gap": 9.471174825762773,
				"focus": -0.7425178722082633
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
					-23.194656075769274,
					129.50352001787041
				]
			]
		},
		{
			"type": "text",
			"version": 31,
			"versionNonce": 616157042,
			"isDeleted": false,
			"id": "1saQwPVe",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -431.7537957606129,
			"y": 2472.968904913725,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 298.4758605957031,
			"height": 45,
			"seed": 1799362862,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "4lKBbfZ6mz6K5xwUKM3C1",
					"type": "arrow"
				}
			],
			"updated": 1693068881407,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "refundFullMoney()",
			"rawText": "refundFullMoney()",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "refundFullMoney()",
			"lineHeight": 1.25,
			"baseline": 32
		},
		{
			"type": "arrow",
			"version": 58,
			"versionNonce": 1116833902,
			"isDeleted": false,
			"id": "4lKBbfZ6mz6K5xwUKM3C1",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -387.8318386405259,
			"y": 2391.2077422466377,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 3.399209554425056,
			"height": 73.4497206451124,
			"seed": 2058585134,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1693134355325,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "tkwgFcuUz980ocUx-W7OL",
				"gap": 12.401401868225548,
				"focus": 0.13242286724601635
			},
			"endBinding": {
				"elementId": "1saQwPVe",
				"gap": 8.311442021974926,
				"focus": -0.7329098476607137
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
					-3.399209554425056,
					73.4497206451124
				]
			]
		},
		{
			"type": "arrow",
			"version": 83,
			"versionNonce": 727762158,
			"isDeleted": false,
			"id": "E4UHnZMt_6FO-tpKu63ID",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 104.519098095679,
			"y": 2382.0048828345666,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 13.560915366858552,
			"height": 97.60523952330777,
			"seed": 1731422642,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1693134355326,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "5EF41dO5cDptKyn1NAywq",
				"gap": 6.079118909540284,
				"focus": 0.04025875574414816
			},
			"endBinding": {
				"elementId": "V9S8uNsh",
				"gap": 5.8564335184191805,
				"focus": -0.24288272673983716
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
					-13.560915366858552,
					97.60523952330777
				]
			]
		},
		{
			"type": "text",
			"version": 78,
			"versionNonce": 1321674734,
			"isDeleted": false,
			"id": "V9S8uNsh",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -36.82404136597847,
			"y": 2485.4665558762936,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 329.1478271484375,
			"height": 45,
			"seed": 1612656878,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "E4UHnZMt_6FO-tpKu63ID",
					"type": "arrow"
				}
			],
			"updated": 1693069050774,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "dispenseItem(code)",
			"rawText": "dispenseItem(code)",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "dispenseItem(code)",
			"lineHeight": 1.25,
			"baseline": 32
		},
		{
			"type": "arrow",
			"version": 38,
			"versionNonce": 1485454510,
			"isDeleted": false,
			"id": "pqx70_1R50jFEHbxsqwxK",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2142.1903348915184,
			"y": 1831.0960972113803,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 229.16666666666606,
			"height": 1.38885498046875,
			"seed": 521324594,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1693134355329,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "4VkNprePekffGKV4CuHrh",
				"gap": 5.633441811318789,
				"focus": -0.4657212674714505
			},
			"endBinding": {
				"elementId": "HYe8n3Yl",
				"gap": 6.11124674479106,
				"focus": -0.11837345479139176
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
					229.16666666666606,
					-1.38885498046875
				]
			]
		},
		{
			"type": "text",
			"version": 49,
			"versionNonce": 2032836334,
			"isDeleted": false,
			"id": "HYe8n3Yl",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2377.4682483029756,
			"y": 1803.3183872504428,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 350.6759033203125,
			"height": 45,
			"seed": 1231714674,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "pqx70_1R50jFEHbxsqwxK",
					"type": "arrow"
				}
			],
			"updated": 1693109330909,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "addItem(item, code)",
			"rawText": "addItem(item, code)",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "addItem(item, code)",
			"lineHeight": 1.25,
			"baseline": 32
		},
		{
			"type": "arrow",
			"version": 73,
			"versionNonce": 700085998,
			"isDeleted": false,
			"id": "shoP5RhvssGVDhi7LHhrl",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2147.3411963591525,
			"y": 1894.3335184205423,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 218.88883463541697,
			"height": 0.00004069010424245789,
			"seed": 345280814,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1693134355329,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "4VkNprePekffGKV4CuHrh",
				"gap": 10.784303278952848,
				"focus": -0.010033976719510685
			},
			"endBinding": {
				"elementId": "gNyTiIzi",
				"gap": 8.444498697916515,
				"focus": -0.13579883478198293
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
					218.88883463541697,
					-0.00004069010424245789
				]
			]
		},
		{
			"type": "text",
			"version": 49,
			"versionNonce": 1133007026,
			"isDeleted": false,
			"id": "gNyTiIzi",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2374.674529692486,
			"y": 1868.777976428355,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 245.8079071044922,
			"height": 45,
			"seed": 1733815090,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "shoP5RhvssGVDhi7LHhrl",
					"type": "arrow"
				}
			],
			"updated": 1693109362248,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "getItem(code)",
			"rawText": "getItem(code)",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "getItem(code)",
			"lineHeight": 1.25,
			"baseline": 32
		},
		{
			"type": "arrow",
			"version": 119,
			"versionNonce": 1432971566,
			"isDeleted": false,
			"id": "bfcv3TKmRBE591D2Rr3kH",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2149.5291611721177,
			"y": 1982.529303454463,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 228.125,
			"height": 1.679117651978686,
			"seed": 1600088690,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1693134355330,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "4VkNprePekffGKV4CuHrh",
				"gap": 12.972268091918068,
				"focus": 0.6626828841511637
			},
			"endBinding": {
				"elementId": "czq6Sodj",
				"gap": 9.375,
				"focus": 0.29274289897288336
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
					228.125,
					-1.679117651978686
				]
			]
		},
		{
			"type": "text",
			"version": 77,
			"versionNonce": 1171027886,
			"isDeleted": false,
			"id": "czq6Sodj",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2387.0291611721177,
			"y": 1963.6987518817764,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 449.171875,
			"height": 45,
			"seed": 397880626,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "bfcv3TKmRBE591D2Rr3kH",
					"type": "arrow"
				}
			],
			"updated": 1693109534782,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "updateSoldOutItem(code)",
			"rawText": "updateSoldOutItem(code)",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "updateSoldOutItem(code)",
			"lineHeight": 1.25,
			"baseline": 32
		},
		{
			"type": "arrow",
			"version": 54,
			"versionNonce": 1273532398,
			"isDeleted": false,
			"id": "qnWfmyXs62AV2rmp86Yom",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2180.7065228458177,
			"y": 2293.772662264165,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 276.1905343191961,
			"height": 1.19049072265625,
			"seed": 267992498,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1693134355331,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "c2Ib2u-lPAJoZqhkxRaVH",
				"gap": 11.470084071501333,
				"focus": -0.40594647042570814
			},
			"endBinding": {
				"elementId": "hrlOW0m9",
				"gap": 2.381068638393117,
				"focus": 0.02592407780811668
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
					276.1905343191961,
					-1.19049072265625
				]
			]
		},
		{
			"type": "text",
			"version": 36,
			"versionNonce": 1099413042,
			"isDeleted": false,
			"id": "hrlOW0m9",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2459.278125803407,
			"y": 2269.9631529868216,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 329.65185546875,
			"height": 45,
			"seed": 1802783986,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "qnWfmyXs62AV2rmp86Yom",
					"type": "arrow"
				}
			],
			"updated": 1693109614476,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "setters & getters",
			"rawText": "setters & getters",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "setters & getters",
			"lineHeight": 1.25,
			"baseline": 32
		},
		{
			"type": "arrow",
			"version": 31,
			"versionNonce": 955768302,
			"isDeleted": false,
			"id": "dAUjC9lDjF-Yv4TLkA_Va",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 770.2956256528,
			"y": 2042.5194300430976,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 3.125,
			"height": 147.91664123535156,
			"seed": 479301678,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1693134355328,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "9ELL9gTEMvRnyhxrGJE4V",
				"gap": 18.29237375468074,
				"focus": -0.05627509051373
			},
			"endBinding": {
				"elementId": "6lOsR6bp",
				"gap": 5.2083587646484375,
				"focus": -0.08866949496199315
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
					3.125,
					147.91664123535156
				]
			]
		},
		{
			"type": "text",
			"version": 72,
			"versionNonce": 1291890222,
			"isDeleted": false,
			"id": "6lOsR6bp",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 623.8372668881515,
			"y": 2195.6444300430976,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 329.65185546875,
			"height": 45,
			"seed": 1795914478,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "dAUjC9lDjF-Yv4TLkA_Va",
					"type": "arrow"
				}
			],
			"updated": 1693109689761,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "getters & setters",
			"rawText": "getters & setters",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "getters & setters",
			"lineHeight": 1.25,
			"baseline": 32
		}
	],
	"appState": {
		"theme": "light",
		"viewBackgroundColor": "#ffffff",
		"currentItemStrokeColor": "#1971c2",
		"currentItemBackgroundColor": "transparent",
		"currentItemFillStyle": "hachure",
		"currentItemStrokeWidth": 1,
		"currentItemStrokeStyle": "solid",
		"currentItemRoughness": 1,
		"currentItemOpacity": 100,
		"currentItemFontFamily": 1,
		"currentItemFontSize": 36,
		"currentItemTextAlign": "left",
		"currentItemStartArrowhead": null,
		"currentItemEndArrowhead": "arrow",
		"scrollX": 847.6474415532161,
		"scrollY": -346.5126654521803,
		"zoom": {
			"value": 0.35
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