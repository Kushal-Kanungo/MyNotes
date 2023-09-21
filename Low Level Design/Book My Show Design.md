---

excalidraw-plugin: parsed
tags: [excalidraw]

---
==⚠  Switch to EXCALIDRAW VIEW in the MORE OPTIONS menu of this document. ⚠==


# Text Elements
Desgin a system for online ticket booking ^R2RvzTay

like : bookMyShow ^Q8vD8H74

Requirements

1. Display all cinemas according to the selected city.

2. Cinemas can be multiplex, Cinema can have multiple halls and each hall can run one movie at a time.

3. Each day one movie can have multiple shows.

4. User should be able to search movies by their title, language, release date, and city name.

5. On selecting the movie, the system should display cinemas running that movie, cinemas can be filtered based on selected city.

6. User should be able to select the cinema and book the ticket.

7. System should redirect to sitting arrangement and user should be able to select the seats.

8. User should be able to complete the payment ^5SZcroTq

Use case Diagram ^aL6UiCaV

City ^ONwyKCBS

Cinema -> hall ^XrYCZqRb

Movie ^hIf0jwAS

Movie Time ^zTtzeVnj

Seat ^uvNTxqoO

Payment ^hzLViWCm

1. Seats should be distinguishable between occupied and vacant.
2. Same seat cannot be booked by multiple users.
3. User should be able to cancel the ticket. ^A1IPwmo3

Actors
users, front_desk_officer, admin, system ^n3IPN9FI

Movie

-int id
- String name
- duration
- other detailes
 ^eBu6i7Ex

setters & getters ^6nZsKVaP

Show

- int showId
- Movie movie
- Screen screen
- DateTime startTime
- List<int> bookedSeatIds
 ^0C7OCMU8

has a ^IzbpWTDJ

Booking

- show
-List<Seat> bookedSeats
- Payment payment
 ^YKgotilZ

has a ^FLj02T5Z

Payment
- int paymentId
- double amount
- otherDetails

 ^HfViIZu6

has a ^JhPb3Zwb

Screen

- screenId
- List<Seats> seats ^qi6oOiiO

Seats

- int seatId
- seatType type
 ^FmOfgXh3

Enum SeatTypes

- Premium
- Silver
- Gold
 ^WlKL1y6H

has a(list) ^XxcllEtC

Theatre

- int theatreId
- List<Screen> screens
- List <Shows> shows ^lLvQKjGq

has a(list) ^WCwWS6px

has a(list)  ^21MDfVpl

TheatreController

- unordredMap <City, List<Theatre>>
- List<Theatre> allTheatre ^xGrM0669

addTheatre(city, theatre) ^ldcsEras

getShow(movie, City) -> theatreVsShows ^YFxj09Vi

MovieController

- unordredMap <City, List<Movies>>
- List<Theatre> allMovies ^BZaMIjho

addMovie(city, movie) ^WV5acuqG

getMovieByCity(movieName) ^c8JBO153

getShows() -> List<shows> ^XG8XW5HB

Service ^CvC8DK35

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
			"version": 125,
			"versionNonce": 2090019314,
			"isDeleted": false,
			"id": "R2RvzTay",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -490.0780944824219,
			"y": -242.42185974121094,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 363.515625,
			"height": 23,
			"seed": 1422003918,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693117276806,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 2,
			"text": "Desgin a system for online ticket booking",
			"rawText": "Desgin a system for online ticket booking",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Desgin a system for online ticket booking",
			"lineHeight": 1.15,
			"baseline": 18
		},
		{
			"type": "text",
			"version": 95,
			"versionNonce": 688006702,
			"isDeleted": false,
			"id": "Q8vD8H74",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -489.2447509765625,
			"y": -219.2551727294922,
			"strokeColor": "#e03131",
			"backgroundColor": "transparent",
			"width": 166.73828125,
			"height": 23,
			"seed": 1341619794,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693117276806,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 2,
			"text": "like : bookMyShow",
			"rawText": "like : bookMyShow",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "like : bookMyShow",
			"lineHeight": 1.15,
			"baseline": 18
		},
		{
			"type": "rectangle",
			"version": 625,
			"versionNonce": 2084379570,
			"isDeleted": false,
			"id": "CN87A6pHJPAOvmxrqdERn",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -502.40043032818085,
			"y": -146.93112013075086,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 797,
			"height": 493,
			"seed": 1512515218,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"type": "text",
					"id": "5SZcroTq"
				}
			],
			"updated": 1693117276806,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 1445,
			"versionNonce": 1182347374,
			"isDeleted": false,
			"id": "5SZcroTq",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -497.40043032818085,
			"y": -141.93112013075086,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 780.439453125,
			"height": 483,
			"seed": 1039352014,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693117276806,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 2,
			"text": "Requirements\n\n1. Display all cinemas according to the selected city.\n\n2. Cinemas can be multiplex, Cinema can have multiple halls and each hall can run one \nmovie at a time.\n\n3. Each day one movie can have multiple shows.\n\n4. User should be able to search movies by their title, language, release date, and city \nname.\n\n5. On selecting the movie, the system should display cinemas running that movie, \ncinemas can be filtered based on selected city.\n\n6. User should be able to select the cinema and book the ticket.\n\n7. System should redirect to sitting arrangement and user should be able to select the \nseats.\n\n8. User should be able to complete the payment",
			"rawText": "Requirements\n\n1. Display all cinemas according to the selected city.\n\n2. Cinemas can be multiplex, Cinema can have multiple halls and each hall can run one movie at a time.\n\n3. Each day one movie can have multiple shows.\n\n4. User should be able to search movies by their title, language, release date, and city name.\n\n5. On selecting the movie, the system should display cinemas running that movie, cinemas can be filtered based on selected city.\n\n6. User should be able to select the cinema and book the ticket.\n\n7. System should redirect to sitting arrangement and user should be able to select the seats.\n\n8. User should be able to complete the payment",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": "CN87A6pHJPAOvmxrqdERn",
			"originalText": "Requirements\n\n1. Display all cinemas according to the selected city.\n\n2. Cinemas can be multiplex, Cinema can have multiple halls and each hall can run one movie at a time.\n\n3. Each day one movie can have multiple shows.\n\n4. User should be able to search movies by their title, language, release date, and city name.\n\n5. On selecting the movie, the system should display cinemas running that movie, cinemas can be filtered based on selected city.\n\n6. User should be able to select the cinema and book the ticket.\n\n7. System should redirect to sitting arrangement and user should be able to select the seats.\n\n8. User should be able to complete the payment",
			"lineHeight": 1.15,
			"baseline": 478
		},
		{
			"type": "text",
			"version": 154,
			"versionNonce": 1788364146,
			"isDeleted": false,
			"id": "aL6UiCaV",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -507.64399529621187,
			"y": 446.2667864373907,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 349.566650390625,
			"height": 48.89712241048923,
			"seed": 2145853518,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693129432716,
			"link": null,
			"locked": false,
			"fontSize": 42.51923687868629,
			"fontFamily": 2,
			"text": "Use case Diagram",
			"rawText": "Use case Diagram",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Use case Diagram",
			"lineHeight": 1.15,
			"baseline": 38
		},
		{
			"type": "rectangle",
			"version": 228,
			"versionNonce": 756347566,
			"isDeleted": false,
			"id": "iiJmqcvqpMgidX0nK5MWc",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -524.9168315924662,
			"y": 532.5294559214003,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 244,
			"height": 79,
			"seed": 1850234706,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"type": "text",
					"id": "ONwyKCBS"
				},
				{
					"id": "gHFTHo7uz_7YiCCNkKAS9",
					"type": "arrow"
				}
			],
			"updated": 1693117276806,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 154,
			"versionNonce": 974364077,
			"isDeleted": false,
			"id": "ONwyKCBS",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -437.0628429450053,
			"y": 549.5294559214003,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 68.29202270507812,
			"height": 45,
			"seed": 1026336334,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693192012279,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "City",
			"rawText": "City",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "iiJmqcvqpMgidX0nK5MWc",
			"originalText": "City",
			"lineHeight": 1.25,
			"baseline": 31
		},
		{
			"type": "rectangle",
			"version": 569,
			"versionNonce": 1199467758,
			"isDeleted": false,
			"id": "L8WeaRKVRyHiincWnWt-8",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 226.59812229639203,
			"y": 524.5402340768454,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 276,
			"height": 100,
			"seed": 1758127182,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"type": "text",
					"id": "XrYCZqRb"
				},
				{
					"id": "Rznc9QjJdx66vEHxe7T5_",
					"type": "arrow"
				},
				{
					"id": "bv36CkBYqXnu7IrddgBbd",
					"type": "arrow"
				}
			],
			"updated": 1693117276806,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 566,
			"versionNonce": 1398046925,
			"isDeleted": false,
			"id": "XrYCZqRb",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 242.9180838442436,
			"y": 552.0402340768454,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 243.36007690429688,
			"height": 45,
			"seed": 650455694,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693192012282,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "Cinema -> hall",
			"rawText": "Cinema -> hall",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "L8WeaRKVRyHiincWnWt-8",
			"originalText": "Cinema -> hall",
			"lineHeight": 1.25,
			"baseline": 31
		},
		{
			"type": "arrow",
			"version": 818,
			"versionNonce": 738516781,
			"isDeleted": false,
			"id": "gHFTHo7uz_7YiCCNkKAS9",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -275.48202902071176,
			"y": 569.8474441446754,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 94.4074887369589,
			"height": 1.0115125909694598,
			"seed": 584009042,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693192012284,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "iiJmqcvqpMgidX0nK5MWc",
				"gap": 5.43480257175446,
				"focus": -0.02001202805393075
			},
			"endBinding": {
				"elementId": "FxK8RdR7jx1VaGT7aGX6D",
				"gap": 7.786382634847769,
				"focus": 0.16060196697260498
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
					94.4074887369589,
					-1.0115125909694598
				]
			]
		},
		{
			"type": "rectangle",
			"version": 629,
			"versionNonce": 216052402,
			"isDeleted": false,
			"id": "FxK8RdR7jx1VaGT7aGX6D",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -173.2881576489051,
			"y": 525.5414894714696,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 276,
			"height": 100,
			"seed": 63883790,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"type": "text",
					"id": "hIf0jwAS"
				},
				{
					"id": "gHFTHo7uz_7YiCCNkKAS9",
					"type": "arrow"
				},
				{
					"id": "Rznc9QjJdx66vEHxe7T5_",
					"type": "arrow"
				}
			],
			"updated": 1693117276806,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 660,
			"versionNonce": 2081339373,
			"isDeleted": false,
			"id": "hIf0jwAS",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -82.25016326413947,
			"y": 553.0414894714696,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 93.92401123046875,
			"height": 45,
			"seed": 197548110,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693192012285,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "Movie",
			"rawText": "Movie",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "FxK8RdR7jx1VaGT7aGX6D",
			"originalText": "Movie",
			"lineHeight": 1.25,
			"baseline": 31
		},
		{
			"type": "arrow",
			"version": 752,
			"versionNonce": 534409613,
			"isDeleted": false,
			"id": "Rznc9QjJdx66vEHxe7T5_",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 114.57748771334687,
			"y": 574.2554167522661,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 102.48036807155529,
			"height": 1.841135678152341,
			"seed": 586104210,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693192012284,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "FxK8RdR7jx1VaGT7aGX6D",
				"gap": 11.865645362251968,
				"focus": -0.07581126450837282
			},
			"endBinding": {
				"elementId": "L8WeaRKVRyHiincWnWt-8",
				"gap": 9.540266511489904,
				"focus": -0.08016476394617718
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
					102.48036807155529,
					1.841135678152341
				]
			]
		},
		{
			"type": "rectangle",
			"version": 641,
			"versionNonce": 994519982,
			"isDeleted": false,
			"id": "TNbakte9eA3UnQlFCMTUz",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 629.1174002789952,
			"y": 523.6378159671362,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 276,
			"height": 100,
			"seed": 1948927182,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"type": "text",
					"id": "zTtzeVnj"
				},
				{
					"id": "bv36CkBYqXnu7IrddgBbd",
					"type": "arrow"
				},
				{
					"id": "20-4CZldI6OyMWz89-3If",
					"type": "arrow"
				}
			],
			"updated": 1693117276807,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 651,
			"versionNonce": 1532150541,
			"isDeleted": false,
			"id": "zTtzeVnj",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 671.5013800763585,
			"y": 551.1378159671362,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 191.23204040527344,
			"height": 45,
			"seed": 1080326926,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693192012288,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "Movie Time",
			"rawText": "Movie Time",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "TNbakte9eA3UnQlFCMTUz",
			"originalText": "Movie Time",
			"lineHeight": 1.25,
			"baseline": 31
		},
		{
			"type": "arrow",
			"version": 299,
			"versionNonce": 715862605,
			"isDeleted": false,
			"id": "bv36CkBYqXnu7IrddgBbd",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 516.9143049690597,
			"y": 577.3169590396112,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 95.41812643471087,
			"height": 1.1760293032643858,
			"seed": 547335502,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693192012286,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "L8WeaRKVRyHiincWnWt-8",
				"gap": 14.31618267266765,
				"focus": 0.017396746091920316
			},
			"endBinding": {
				"elementId": "TNbakte9eA3UnQlFCMTUz",
				"gap": 16.78496887522465,
				"focus": -0.13080826329919662
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
					95.41812643471087,
					1.1760293032643858
				]
			]
		},
		{
			"type": "rectangle",
			"version": 80,
			"versionNonce": 1244960754,
			"isDeleted": false,
			"id": "orlYKlTylhohwlEfHlgcR",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1091.6505537618805,
			"y": 522.2014849178779,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 230,
			"height": 98,
			"seed": 742613390,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"type": "text",
					"id": "uvNTxqoO"
				},
				{
					"id": "20-4CZldI6OyMWz89-3If",
					"type": "arrow"
				},
				{
					"id": "iqHil0xWaIvvCqRlbbdo0",
					"type": "arrow"
				}
			],
			"updated": 1693117276807,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 39,
			"versionNonce": 2080449069,
			"isDeleted": false,
			"id": "uvNTxqoO",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1163.6845350851227,
			"y": 548.7014849178779,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 85.93203735351562,
			"height": 45,
			"seed": 1552806222,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693192012290,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "Seat",
			"rawText": "Seat",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "orlYKlTylhohwlEfHlgcR",
			"originalText": "Seat",
			"lineHeight": 1.25,
			"baseline": 31
		},
		{
			"type": "arrow",
			"version": 147,
			"versionNonce": 394320237,
			"isDeleted": false,
			"id": "20-4CZldI6OyMWz89-3If",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 910.2843321538985,
			"y": 572.3802162435709,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 165.38470928485572,
			"height": 3.0464380559085384,
			"seed": 780507346,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693192012289,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "TNbakte9eA3UnQlFCMTUz",
				"gap": 5.166931874903298,
				"focus": -0.07412696774686335
			},
			"endBinding": {
				"elementId": "orlYKlTylhohwlEfHlgcR",
				"gap": 15.981512323126253,
				"focus": -0.1298534012959957
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
					165.38470928485572,
					3.0464380559085384
				]
			]
		},
		{
			"type": "rectangle",
			"version": 71,
			"versionNonce": 487547502,
			"isDeleted": false,
			"id": "rxYeCMPhr4bW8gl8mKQLv",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1448.0545965064525,
			"y": 519.7516102986897,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 279,
			"height": 100,
			"seed": 206514062,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"type": "text",
					"id": "hzLViWCm"
				},
				{
					"id": "iqHil0xWaIvvCqRlbbdo0",
					"type": "arrow"
				}
			],
			"updated": 1693117276807,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 27,
			"versionNonce": 1981168365,
			"isDeleted": false,
			"id": "hzLViWCm",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1515.3925710547924,
			"y": 547.2516102986897,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 144.3240509033203,
			"height": 45,
			"seed": 1347932498,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693192012292,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "Payment",
			"rawText": "Payment",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "rxYeCMPhr4bW8gl8mKQLv",
			"originalText": "Payment",
			"lineHeight": 1.25,
			"baseline": 31
		},
		{
			"type": "arrow",
			"version": 90,
			"versionNonce": 1297503373,
			"isDeleted": false,
			"id": "iqHil0xWaIvvCqRlbbdo0",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1331.5554660078537,
			"y": 568.7712290215338,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 107.57579456676149,
			"height": 0,
			"seed": 1100232846,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693192012292,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "orlYKlTylhohwlEfHlgcR",
				"gap": 9.904912245973264,
				"focus": -0.049597059109062834
			},
			"endBinding": {
				"elementId": "rxYeCMPhr4bW8gl8mKQLv",
				"gap": 8.9233359318373,
				"focus": 0.019607625543117138
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
					107.57579456676149,
					0
				]
			]
		},
		{
			"type": "rectangle",
			"version": 234,
			"versionNonce": 1302037810,
			"isDeleted": false,
			"id": "-F-hNr7Te2BYb2mbZn6X2",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 335.85466307408,
			"y": -145.94433385119464,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffec99",
			"width": 952,
			"height": 488,
			"seed": 926838094,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"type": "text",
					"id": "A1IPwmo3"
				}
			],
			"updated": 1693117276807,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 211,
			"versionNonce": 263200494,
			"isDeleted": false,
			"id": "A1IPwmo3",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 340.85466307408,
			"y": -140.94433385119464,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffec99",
			"width": 926.666015625,
			"height": 165.6,
			"seed": 585938126,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693117276807,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 2,
			"text": "1. Seats should be distinguishable between occupied and \nvacant.\n2. Same seat cannot be booked by multiple users.\n3. User should be able to cancel the ticket.",
			"rawText": "1. Seats should be distinguishable between occupied and vacant.\n2. Same seat cannot be booked by multiple users.\n3. User should be able to cancel the ticket.",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": "-F-hNr7Te2BYb2mbZn6X2",
			"originalText": "1. Seats should be distinguishable between occupied and vacant.\n2. Same seat cannot be booked by multiple users.\n3. User should be able to cancel the ticket.",
			"lineHeight": 1.15,
			"baseline": 157
		},
		{
			"type": "text",
			"version": 183,
			"versionNonce": 437784306,
			"isDeleted": false,
			"id": "n3IPN9FI",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -474.5681521257196,
			"y": 744.6960605706495,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffec99",
			"width": 926.04541015625,
			"height": 119.16363636363631,
			"seed": 1105478510,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693117276807,
			"link": null,
			"locked": false,
			"fontSize": 51.81027667984188,
			"fontFamily": 2,
			"text": "Actors\nusers, front_desk_officer, admin, system",
			"rawText": "Actors\nusers, front_desk_officer, admin, system",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Actors\nusers, front_desk_officer, admin, system",
			"lineHeight": 1.15,
			"baseline": 107
		},
		{
			"type": "rectangle",
			"version": 122,
			"versionNonce": 1420473262,
			"isDeleted": false,
			"id": "L1li4lyYUcXUsLCT_19PJ",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 257.1374431409299,
			"y": 2191.3250044635597,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffec99",
			"width": 631,
			"height": 325,
			"seed": 996685106,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"type": "text",
					"id": "eBu6i7Ex"
				},
				{
					"id": "12pXdd6MshoTWV8R9B8bl",
					"type": "arrow"
				},
				{
					"id": "6_VxGNxZ18D14pKdcSp45",
					"type": "arrow"
				}
			],
			"updated": 1693118732945,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 122,
			"versionNonce": 910501389,
			"isDeleted": false,
			"id": "eBu6i7Ex",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 430.0594096936643,
			"y": 2196.3250044635597,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffec99",
			"width": 285.15606689453125,
			"height": 315,
			"seed": 1452881646,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693192012298,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "Movie\n\n-int id\n- String name\n- duration\n- other detailes\n",
			"rawText": "Movie\n\n-int id\n- String name\n- duration\n- other detailes\n",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "L1li4lyYUcXUsLCT_19PJ",
			"originalText": "Movie\n\n-int id\n- String name\n- duration\n- other detailes\n",
			"lineHeight": 1.25,
			"baseline": 301
		},
		{
			"type": "arrow",
			"version": 160,
			"versionNonce": 516576589,
			"isDeleted": false,
			"id": "12pXdd6MshoTWV8R9B8bl",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 896.5881062192739,
			"y": 2265.5605513895152,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffec99",
			"width": 171.23017810639863,
			"height": 2.7871151016929616,
			"seed": 427385582,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693192012297,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "L1li4lyYUcXUsLCT_19PJ",
				"gap": 8.45066307834395,
				"focus": -0.49338365130877143
			},
			"endBinding": {
				"elementId": "6nZsKVaP",
				"gap": 11.111043294270758,
				"focus": -0.14542265846606262
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
					171.23017810639863,
					-2.7871151016929616
				]
			]
		},
		{
			"type": "text",
			"version": 114,
			"versionNonce": 1888647794,
			"isDeleted": false,
			"id": "6nZsKVaP",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1078.9293276199433,
			"y": 2233.7475460522473,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffec99",
			"width": 329.652099609375,
			"height": 45,
			"seed": 1492683950,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "12pXdd6MshoTWV8R9B8bl",
					"type": "arrow"
				}
			],
			"updated": 1693117276807,
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
			"baseline": 31
		},
		{
			"type": "rectangle",
			"version": 189,
			"versionNonce": 1849871278,
			"isDeleted": false,
			"id": "VLR5w2ytpOp6eXwwKIleI",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -599.6561441439975,
			"y": 2139.5357165708,
			"strokeColor": "#2f9e44",
			"backgroundColor": "#b2f2bb",
			"width": 519,
			"height": 415,
			"seed": 1696793586,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"type": "text",
					"id": "0C7OCMU8"
				},
				{
					"id": "6_VxGNxZ18D14pKdcSp45",
					"type": "arrow"
				},
				{
					"id": "wjvo3E2RfFDzJjYGAW8jy",
					"type": "arrow"
				},
				{
					"id": "qyqmuwuSQkuu1zwYUnD8O",
					"type": "arrow"
				}
			],
			"updated": 1693117602843,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 265,
			"versionNonce": 645871501,
			"isDeleted": false,
			"id": "0C7OCMU8",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -573.0942239779819,
			"y": 2167.0357165708,
			"strokeColor": "#2f9e44",
			"backgroundColor": "#b2f2bb",
			"width": 465.87615966796875,
			"height": 360,
			"seed": 1151449838,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693192012303,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "Show\n\n- int showId\n- Movie movie\n- Screen screen\n- DateTime startTime\n- List<int> bookedSeatIds\n",
			"rawText": "Show\n\n- int showId\n- Movie movie\n- Screen screen\n- DateTime startTime\n- List<int> bookedSeatIds\n",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "VLR5w2ytpOp6eXwwKIleI",
			"originalText": "Show\n\n- int showId\n- Movie movie\n- Screen screen\n- DateTime startTime\n- List<int> bookedSeatIds\n",
			"lineHeight": 1.25,
			"baseline": 346
		},
		{
			"type": "arrow",
			"version": 208,
			"versionNonce": 1278139501,
			"isDeleted": false,
			"id": "6_VxGNxZ18D14pKdcSp45",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -71.07426239736094,
			"y": 2305.364554611808,
			"strokeColor": "#2f9e44",
			"backgroundColor": "#b2f2bb",
			"width": 308.333282470703,
			"height": 2.8380575016003604,
			"seed": 1986845422,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"type": "text",
					"id": "IzbpWTDJ"
				}
			],
			"updated": 1693192012300,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "VLR5w2ytpOp6eXwwKIleI",
				"gap": 9.581881746636498,
				"focus": -0.18673437769984677
			},
			"endBinding": {
				"elementId": "L1li4lyYUcXUsLCT_19PJ",
				"gap": 19.878423067587846,
				"focus": 0.3288039854643337
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
					308.333282470703,
					-2.8380575016003604
				]
			]
		},
		{
			"type": "text",
			"version": 45,
			"versionNonce": 1829242354,
			"isDeleted": false,
			"id": "IzbpWTDJ",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 47.03939269297098,
			"y": 2268.3590662794068,
			"strokeColor": "#2f9e44",
			"backgroundColor": "#b2f2bb",
			"width": 103.35603332519531,
			"height": 45,
			"seed": 848976498,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693117276807,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "has a",
			"rawText": "has a",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "6_VxGNxZ18D14pKdcSp45",
			"originalText": "has a",
			"lineHeight": 1.25,
			"baseline": 31
		},
		{
			"type": "rectangle",
			"version": 267,
			"versionNonce": 1272515118,
			"isDeleted": false,
			"id": "v3DDUGYtk_UJXvM5fpxb9",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1600.6012507957475,
			"y": 2123.5339473518547,
			"strokeColor": "#1971c2",
			"backgroundColor": "#a5d8ff",
			"width": 606,
			"height": 280,
			"seed": 234548846,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"type": "text",
					"id": "YKgotilZ"
				},
				{
					"id": "wjvo3E2RfFDzJjYGAW8jy",
					"type": "arrow"
				},
				{
					"id": "ypk9_m_2Mp7AWtQ0OVKxN",
					"type": "arrow"
				}
			],
			"updated": 1693117276807,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 311,
			"versionNonce": 2078009005,
			"isDeleted": false,
			"id": "YKgotilZ",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1521.935326723482,
			"y": 2128.5339473518547,
			"strokeColor": "#1971c2",
			"backgroundColor": "#b2f2bb",
			"width": 448.66815185546875,
			"height": 270,
			"seed": 511312174,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693192012307,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "Booking\n\n- show\n-List<Seat> bookedSeats\n- Payment payment\n",
			"rawText": "Booking\n\n- show\n-List<Seat> bookedSeats\n- Payment payment\n",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "v3DDUGYtk_UJXvM5fpxb9",
			"originalText": "Booking\n\n- show\n-List<Seat> bookedSeats\n- Payment payment\n",
			"lineHeight": 1.25,
			"baseline": 256
		},
		{
			"type": "arrow",
			"version": 177,
			"versionNonce": 506117613,
			"isDeleted": false,
			"id": "wjvo3E2RfFDzJjYGAW8jy",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -987.3535100774914,
			"y": 2264.2402483993246,
			"strokeColor": "#1971c2",
			"backgroundColor": "#a5d8ff",
			"width": 374.19190192945075,
			"height": 4.680451474118854,
			"seed": 1457885810,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"type": "text",
					"id": "FLj02T5Z"
				}
			],
			"updated": 1693192012305,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "v3DDUGYtk_UJXvM5fpxb9",
				"gap": 7.247740718256182,
				"focus": -0.022076134417837907
			},
			"endBinding": {
				"elementId": "VLR5w2ytpOp6eXwwKIleI",
				"gap": 13.50546400404312,
				"focus": 0.3544563992657366
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
					374.19190192945075,
					4.680451474118854
				]
			]
		},
		{
			"type": "text",
			"version": 13,
			"versionNonce": 1664135538,
			"isDeleted": false,
			"id": "FLj02T5Z",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -954.9911279400771,
			"y": 2244.143879071966,
			"strokeColor": "#1971c2",
			"backgroundColor": "#a5d8ff",
			"width": 103.35603332519531,
			"height": 45,
			"seed": 144074734,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693117276807,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "has a",
			"rawText": "has a",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "wjvo3E2RfFDzJjYGAW8jy",
			"originalText": "has a",
			"lineHeight": 1.25,
			"baseline": 31
		},
		{
			"type": "rectangle",
			"version": 141,
			"versionNonce": 713217710,
			"isDeleted": false,
			"id": "_5kJU3N2aiNiLMuJxscRI",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -2667.014416011835,
			"y": 2092.7982527032987,
			"strokeColor": "#f08c00",
			"backgroundColor": "#ffec99",
			"width": 610,
			"height": 350,
			"seed": 1854041262,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"type": "text",
					"id": "HfViIZu6"
				},
				{
					"id": "ypk9_m_2Mp7AWtQ0OVKxN",
					"type": "arrow"
				}
			],
			"updated": 1693117276807,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 171,
			"versionNonce": 1080680301,
			"isDeleted": false,
			"id": "HfViIZu6",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -2503.7464716758973,
			"y": 2132.7982527032987,
			"strokeColor": "#f08c00",
			"backgroundColor": "#ffec99",
			"width": 283.464111328125,
			"height": 270,
			"seed": 1845430066,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693192012310,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "Payment\n- int paymentId\n- double amount\n- otherDetails\n\n",
			"rawText": "Payment\n- int paymentId\n- double amount\n- otherDetails\n\n",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "_5kJU3N2aiNiLMuJxscRI",
			"originalText": "Payment\n- int paymentId\n- double amount\n- otherDetails\n\n",
			"lineHeight": 1.25,
			"baseline": 256
		},
		{
			"type": "arrow",
			"version": 84,
			"versionNonce": 2120517901,
			"isDeleted": false,
			"id": "ypk9_m_2Mp7AWtQ0OVKxN",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1620.029844525222,
			"y": 2240.7128059867246,
			"strokeColor": "#f08c00",
			"backgroundColor": "#ffec99",
			"width": 419.444376627604,
			"height": 3.3390889027414232,
			"seed": 734853486,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"type": "text",
					"id": "JhPb3Zwb"
				}
			],
			"updated": 1693192012308,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "v3DDUGYtk_UJXvM5fpxb9",
				"gap": 19.428593729474414,
				"focus": 0.17827074829020018
			},
			"endBinding": {
				"elementId": "_5kJU3N2aiNiLMuJxscRI",
				"gap": 17.540194859008807,
				"focus": -0.1193650101642223
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
					-419.444376627604,
					3.3390889027414232
				]
			]
		},
		{
			"type": "text",
			"version": 7,
			"versionNonce": 415530226,
			"isDeleted": false,
			"id": "JhPb3Zwb",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1879.3466856507102,
			"y": 2216.0760425912267,
			"strokeColor": "#f08c00",
			"backgroundColor": "#ffec99",
			"width": 103.35603332519531,
			"height": 45,
			"seed": 52382898,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693117276807,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "has a",
			"rawText": "has a",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "ypk9_m_2Mp7AWtQ0OVKxN",
			"originalText": "has a",
			"lineHeight": 1.25,
			"baseline": 31
		},
		{
			"type": "rectangle",
			"version": 55,
			"versionNonce": 1048101810,
			"isDeleted": false,
			"id": "gPjUgymeJAFKONCrtCKvz",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -755.2738957552957,
			"y": 2900.1499697288136,
			"strokeColor": "#099268",
			"backgroundColor": "#96f2d7",
			"width": 563,
			"height": 393,
			"seed": 1086778734,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"type": "text",
					"id": "qi6oOiiO"
				},
				{
					"id": "oWF-bi7AqnnNkL8nljf7X",
					"type": "arrow"
				},
				{
					"id": "CqEI3LPAcKPxH8yWWra-H",
					"type": "arrow"
				}
			],
			"updated": 1693117592068,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 73,
			"versionNonce": 1851071117,
			"isDeleted": false,
			"id": "qi6oOiiO",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -657.7699589877176,
			"y": 3006.6499697288136,
			"strokeColor": "#099268",
			"backgroundColor": "#96f2d7",
			"width": 367.99212646484375,
			"height": 180,
			"seed": 1699511154,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693192012312,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "Screen\n\n- screenId\n- List<Seats> seats",
			"rawText": "Screen\n\n- screenId\n- List<Seats> seats",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "gPjUgymeJAFKONCrtCKvz",
			"originalText": "Screen\n\n- screenId\n- List<Seats> seats",
			"lineHeight": 1.25,
			"baseline": 166
		},
		{
			"type": "rectangle",
			"version": 72,
			"versionNonce": 754901742,
			"isDeleted": false,
			"id": "1yA4fTSQ4WZqEA609MoPs",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 128.81987023010345,
			"y": 2926.479185342613,
			"strokeColor": "#c2255c",
			"backgroundColor": "#fcc2d7",
			"width": 599,
			"height": 370,
			"seed": 490578222,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"type": "text",
					"id": "FmOfgXh3"
				},
				{
					"id": "oWF-bi7AqnnNkL8nljf7X",
					"type": "arrow"
				},
				{
					"id": "4eWyAk1h09InRoFCxHI4q",
					"type": "arrow"
				}
			],
			"updated": 1693117516939,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 60,
			"versionNonce": 1186507181,
			"isDeleted": false,
			"id": "FmOfgXh3",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 282.15983605041595,
			"y": 2998.979185342613,
			"strokeColor": "#c2255c",
			"backgroundColor": "#fcc2d7",
			"width": 292.320068359375,
			"height": 225,
			"seed": 2030597870,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693192012315,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "Seats\n\n- int seatId\n- seatType type\n",
			"rawText": "Seats\n\n- int seatId\n- seatType type\n",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "1yA4fTSQ4WZqEA609MoPs",
			"originalText": "Seats\n\n- int seatId\n- seatType type\n",
			"lineHeight": 1.25,
			"baseline": 211
		},
		{
			"type": "rectangle",
			"version": 223,
			"versionNonce": 1296061742,
			"isDeleted": false,
			"id": "T7ZtnL5BzroQh_jno5_pk",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1164.2754627197537,
			"y": 2767.9864718657695,
			"strokeColor": "#c2255c",
			"backgroundColor": "#fcc2d7",
			"width": 599,
			"height": 370,
			"seed": 72067506,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"type": "text",
					"id": "WlKL1y6H"
				},
				{
					"id": "4eWyAk1h09InRoFCxHI4q",
					"type": "arrow"
				}
			],
			"updated": 1693117516939,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 244,
			"versionNonce": 1462887021,
			"isDeleted": false,
			"id": "WlKL1y6H",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1318.2454029053006,
			"y": 2817.9864718657695,
			"strokeColor": "#c2255c",
			"backgroundColor": "#fcc2d7",
			"width": 291.06011962890625,
			"height": 270,
			"seed": 1078961010,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693192012317,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "Enum SeatTypes\n\n- Premium\n- Silver\n- Gold\n",
			"rawText": "Enum SeatTypes\n\n- Premium\n- Silver\n- Gold\n",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "T7ZtnL5BzroQh_jno5_pk",
			"originalText": "Enum SeatTypes\n\n- Premium\n- Silver\n- Gold\n",
			"lineHeight": 1.25,
			"baseline": 256
		},
		{
			"type": "arrow",
			"version": 73,
			"versionNonce": 1464615149,
			"isDeleted": false,
			"id": "oWF-bi7AqnnNkL8nljf7X",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -176.4895315091082,
			"y": 3076.608231567707,
			"strokeColor": "#c2255c",
			"backgroundColor": "#fcc2d7",
			"width": 290.74069552951386,
			"height": 1.2397125346410576,
			"seed": 901536050,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"type": "text",
					"id": "XxcllEtC"
				}
			],
			"updated": 1693192012313,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "gPjUgymeJAFKONCrtCKvz",
				"gap": 15.784364246187465,
				"focus": -0.09496253984682675
			},
			"endBinding": {
				"elementId": "1yA4fTSQ4WZqEA609MoPs",
				"gap": 14.56870620969778,
				"focus": 0.20104380328990082
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
					290.74069552951386,
					-1.2397125346410576
				]
			]
		},
		{
			"type": "text",
			"version": 14,
			"versionNonce": 563314,
			"isDeleted": false,
			"id": "XxcllEtC",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -133.30447630620029,
			"y": 3055.489830648912,
			"strokeColor": "#c2255c",
			"backgroundColor": "#fcc2d7",
			"width": 187.7040557861328,
			"height": 45,
			"seed": 76909618,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693117511130,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "has a(list)",
			"rawText": "has a(list)",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "oWF-bi7AqnnNkL8nljf7X",
			"originalText": "has a(list)",
			"lineHeight": 1.25,
			"baseline": 31
		},
		{
			"type": "arrow",
			"version": 52,
			"versionNonce": 1991306253,
			"isDeleted": false,
			"id": "4eWyAk1h09InRoFCxHI4q",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 740.1771351575585,
			"y": 3168.7305939952657,
			"strokeColor": "#c2255c",
			"backgroundColor": "#fcc2d7",
			"width": 412.96278211805566,
			"height": 246.29631890190922,
			"seed": 649899762,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693192012316,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "1yA4fTSQ4WZqEA609MoPs",
				"gap": 12.357264927455049,
				"focus": 0.668949212534609
			},
			"endBinding": {
				"elementId": "T7ZtnL5BzroQh_jno5_pk",
				"gap": 11.135545444139552,
				"focus": 0.5935203732404685
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
					412.96278211805566,
					-246.29631890190922
				]
			]
		},
		{
			"type": "rectangle",
			"version": 312,
			"versionNonce": 943990706,
			"isDeleted": false,
			"id": "CcHnRwvvxdoZU5jjTxDNz",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -2099.0103559591907,
			"y": 2887.7748201289887,
			"strokeColor": "#c2255c",
			"backgroundColor": "#fcc2d7",
			"width": 767,
			"height": 531,
			"seed": 1092190062,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"type": "text",
					"id": "lLvQKjGq"
				},
				{
					"id": "CqEI3LPAcKPxH8yWWra-H",
					"type": "arrow"
				},
				{
					"id": "qyqmuwuSQkuu1zwYUnD8O",
					"type": "arrow"
				},
				{
					"id": "6mxhrmnFx9rLgCOsn5-q1",
					"type": "arrow"
				}
			],
			"updated": 1693129020486,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 252,
			"versionNonce": 534392259,
			"isDeleted": false,
			"id": "lLvQKjGq",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1915.436442384972,
			"y": 3040.7748201289887,
			"strokeColor": "#c2255c",
			"backgroundColor": "#fcc2d7",
			"width": 399.8521728515625,
			"height": 225,
			"seed": 2145272434,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693192012320,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "Theatre\n\n- int theatreId\n- List<Screen> screens\n- List <Shows> shows",
			"rawText": "Theatre\n\n- int theatreId\n- List<Screen> screens\n- List <Shows> shows",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "CcHnRwvvxdoZU5jjTxDNz",
			"originalText": "Theatre\n\n- int theatreId\n- List<Screen> screens\n- List <Shows> shows",
			"lineHeight": 1.25,
			"baseline": 211
		},
		{
			"type": "arrow",
			"version": 315,
			"versionNonce": 1023741133,
			"isDeleted": false,
			"id": "CqEI3LPAcKPxH8yWWra-H",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1317.9388401946817,
			"y": 3120.91697253195,
			"strokeColor": "#c2255c",
			"backgroundColor": "#fcc2d7",
			"width": 544.3453543526787,
			"height": 78.79970634477013,
			"seed": 448822510,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"type": "text",
					"id": "WCwWS6px"
				}
			],
			"updated": 1693192012318,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "CcHnRwvvxdoZU5jjTxDNz",
				"gap": 14.071515764509058,
				"focus": 0.07848465995285038
			},
			"endBinding": {
				"elementId": "gPjUgymeJAFKONCrtCKvz",
				"gap": 18.319590086707308,
				"focus": 0.41279116631200247
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
					544.3453543526787,
					-78.79970634477013
				]
			]
		},
		{
			"type": "text",
			"version": 12,
			"versionNonce": 559201454,
			"isDeleted": false,
			"id": "WCwWS6px",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1170.5704450705189,
			"y": 3001.399781982016,
			"strokeColor": "#c2255c",
			"backgroundColor": "#fcc2d7",
			"width": 187.7040557861328,
			"height": 45,
			"seed": 1336724142,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693117599339,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "has a(list)",
			"rawText": "has a(list)",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "CqEI3LPAcKPxH8yWWra-H",
			"originalText": "has a(list)",
			"lineHeight": 1.25,
			"baseline": 31
		},
		{
			"type": "arrow",
			"version": 312,
			"versionNonce": 667151149,
			"isDeleted": false,
			"id": "qyqmuwuSQkuu1zwYUnD8O",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1322.105405136088,
			"y": 2942.9624670530106,
			"strokeColor": "#c2255c",
			"backgroundColor": "#fcc2d7",
			"width": 706.8453543526784,
			"height": 396.0096732966108,
			"seed": 1966405358,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"type": "text",
					"id": "21MDfVpl"
				}
			],
			"updated": 1693192012319,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "CcHnRwvvxdoZU5jjTxDNz",
				"gap": 9.904950823102808,
				"focus": 0.021010532387670262
			},
			"endBinding": {
				"elementId": "VLR5w2ytpOp6eXwwKIleI",
				"gap": 15.603906639412003,
				"focus": -0.12975989453075393
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
					706.8453543526784,
					-396.0096732966108
				]
			]
		},
		{
			"type": "text",
			"version": 13,
			"versionNonce": 957988270,
			"isDeleted": false,
			"id": "21MDfVpl",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1102.4870100119251,
			"y": 2657.6498010555024,
			"strokeColor": "#c2255c",
			"backgroundColor": "#fcc2d7",
			"width": 205.7040557861328,
			"height": 45,
			"seed": 1031206898,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693117609153,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "has a(list) ",
			"rawText": "has a(list) ",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "qyqmuwuSQkuu1zwYUnD8O",
			"originalText": "has a(list) ",
			"lineHeight": 1.25,
			"baseline": 31
		},
		{
			"type": "rectangle",
			"version": 398,
			"versionNonce": 1656383730,
			"isDeleted": false,
			"id": "xPYtGlFKUbArUew6N-GWD",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -3381.625142743045,
			"y": 2728.839434978464,
			"strokeColor": "#c2255c",
			"backgroundColor": "#fcc2d7",
			"width": 767,
			"height": 531,
			"seed": 686471982,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"type": "text",
					"id": "xGrM0669"
				},
				{
					"id": "jkIDl4RfeGpqBYSPZksud",
					"type": "arrow"
				},
				{
					"id": "CVdXDcB3fezZEKV9tkT8p",
					"type": "arrow"
				}
			],
			"updated": 1693117996947,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 431,
			"versionNonce": 952746147,
			"isDeleted": false,
			"id": "xGrM0669",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -3327.25526969617,
			"y": 2904.339434978464,
			"strokeColor": "#c2255c",
			"backgroundColor": "#fcc2d7",
			"width": 658.26025390625,
			"height": 180,
			"seed": 1183262062,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693192012323,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "TheatreController\n\n- unordredMap <City, List<Theatre>>\n- List<Theatre> allTheatre",
			"rawText": "TheatreController\n\n- unordredMap <City, List<Theatre>>\n- List<Theatre> allTheatre",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "xPYtGlFKUbArUew6N-GWD",
			"originalText": "TheatreController\n\n- unordredMap <City, List<Theatre>>\n- List<Theatre> allTheatre",
			"lineHeight": 1.25,
			"baseline": 166
		},
		{
			"type": "arrow",
			"version": 256,
			"versionNonce": 678788451,
			"isDeleted": false,
			"id": "jkIDl4RfeGpqBYSPZksud",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -3290.7682524750385,
			"y": 3272.909011072503,
			"strokeColor": "#c2255c",
			"backgroundColor": "#fcc2d7",
			"width": 145.6772574026013,
			"height": 196.79473876953034,
			"seed": 1244167986,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693192012321,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "xPYtGlFKUbArUew6N-GWD",
				"gap": 13.069576094038894,
				"focus": 0.14917272984235852
			},
			"endBinding": {
				"elementId": "ldcsEras",
				"gap": 3.3333646334135665,
				"focus": -0.3473246456280024
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
					-145.6772574026013,
					196.79473876953034
				]
			]
		},
		{
			"type": "text",
			"version": 80,
			"versionNonce": 932262958,
			"isDeleted": false,
			"id": "ldcsEras",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -3605.7571270766666,
			"y": 3473.0371144754467,
			"strokeColor": "#c2255c",
			"backgroundColor": "#fcc2d7",
			"width": 477.125732421875,
			"height": 46.1146983610632,
			"seed": 1152062766,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "jkIDl4RfeGpqBYSPZksud",
					"type": "arrow"
				}
			],
			"updated": 1693118001549,
			"link": null,
			"locked": false,
			"fontSize": 36.89175868885056,
			"fontFamily": 1,
			"text": "addTheatre(city, theatre)",
			"rawText": "addTheatre(city, theatre)",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "addTheatre(city, theatre)",
			"lineHeight": 1.25,
			"baseline": 32
		},
		{
			"type": "arrow",
			"version": 225,
			"versionNonce": 205904131,
			"isDeleted": false,
			"id": "CVdXDcB3fezZEKV9tkT8p",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -2844.3310170994578,
			"y": 3270.3448772083207,
			"strokeColor": "#c2255c",
			"backgroundColor": "#fcc2d7",
			"width": 78.04923330991869,
			"height": 179.00645329402005,
			"seed": 1428950194,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"type": "text",
					"id": "CvC8DK35"
				}
			],
			"updated": 1693192012322,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "xPYtGlFKUbArUew6N-GWD",
				"gap": 10.505442229856271,
				"focus": -0.067003948555474
			},
			"endBinding": {
				"elementId": "YFxj09Vi",
				"gap": 1.5384615384618883,
				"focus": -0.41018444348331057
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
					78.04923330991869,
					179.00645329402005
				]
			]
		},
		{
			"type": "text",
			"version": 18,
			"versionNonce": 15148402,
			"isDeleted": false,
			"id": "CvC8DK35",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -2866.0750501383245,
			"y": 3337.34810385533,
			"strokeColor": "#c2255c",
			"backgroundColor": "#fcc2d7",
			"width": 121.53604125976562,
			"height": 45,
			"seed": 1865006514,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693134843865,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "Service",
			"rawText": "Service",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "CVdXDcB3fezZEKV9tkT8p",
			"originalText": "Service",
			"lineHeight": 1.25,
			"baseline": 31
		},
		{
			"type": "text",
			"version": 92,
			"versionNonce": 1681890226,
			"isDeleted": false,
			"id": "YFxj09Vi",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -2957.1033161354103,
			"y": 3450.889792040802,
			"strokeColor": "#c2255c",
			"backgroundColor": "#fcc2d7",
			"width": 696.240234375,
			"height": 45,
			"seed": 198674734,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "CVdXDcB3fezZEKV9tkT8p",
					"type": "arrow"
				}
			],
			"updated": 1693118003016,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "getShow(movie, City) -> theatreVsShows",
			"rawText": "getShow(movie, City) -> theatreVsShows",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "getShow(movie, City) -> theatreVsShows",
			"lineHeight": 1.25,
			"baseline": 31
		},
		{
			"type": "rectangle",
			"version": 502,
			"versionNonce": 484824370,
			"isDeleted": false,
			"id": "67qkq1ZdJ1JCJJtaW-8-v",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -4176.5339361542265,
			"y": 1809.2180754822139,
			"strokeColor": "#c2255c",
			"backgroundColor": "#fcc2d7",
			"width": 767,
			"height": 531,
			"seed": 530789042,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"type": "text",
					"id": "BZaMIjho"
				},
				{
					"id": "24IjvgaYosz9E63M5PIfF",
					"type": "arrow"
				},
				{
					"id": "gaoN0NpZAR0AIWdpsZeO1",
					"type": "arrow"
				}
			],
			"updated": 1693134909564,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 586,
			"versionNonce": 1280032643,
			"isDeleted": false,
			"id": "BZaMIjho",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -4105.928040158133,
			"y": 1984.7180754822139,
			"strokeColor": "#c2255c",
			"backgroundColor": "#fcc2d7",
			"width": 625.7882080078125,
			"height": 180,
			"seed": 2043546738,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693192012326,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "MovieController\n\n- unordredMap <City, List<Movies>>\n- List<Theatre> allMovies",
			"rawText": "MovieController\n\n- unordredMap <City, List<Movies>>\n- List<Theatre> allMovies",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "67qkq1ZdJ1JCJJtaW-8-v",
			"originalText": "MovieController\n\n- unordredMap <City, List<Movies>>\n- List<Theatre> allMovies",
			"lineHeight": 1.25,
			"baseline": 166
		},
		{
			"type": "arrow",
			"version": 55,
			"versionNonce": 1739568195,
			"isDeleted": false,
			"id": "24IjvgaYosz9E63M5PIfF",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -4069.357612584458,
			"y": 2348.4446402721337,
			"strokeColor": "#c2255c",
			"backgroundColor": "#fcc2d7",
			"width": 189.56988491439324,
			"height": 200.25265040542172,
			"seed": 318556850,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693192012325,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "67qkq1ZdJ1JCJJtaW-8-v",
				"gap": 8.226564789919848,
				"focus": 0.027105714881891268
			},
			"endBinding": {
				"elementId": "WV5acuqG",
				"gap": 5.3333740234375,
				"focus": 0.04786103949098742
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
					-189.56988491439324,
					200.25265040542172
				]
			]
		},
		{
			"type": "text",
			"version": 66,
			"versionNonce": 560697582,
			"isDeleted": false,
			"id": "WV5acuqG",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -4477.834046545951,
			"y": 2554.030664700993,
			"strokeColor": "#c2255c",
			"backgroundColor": "#fcc2d7",
			"width": 365.580078125,
			"height": 45,
			"seed": 2133098610,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "24IjvgaYosz9E63M5PIfF",
					"type": "arrow"
				}
			],
			"updated": 1693118182122,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "addMovie(city, movie)",
			"rawText": "addMovie(city, movie)",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "addMovie(city, movie)",
			"lineHeight": 1.25,
			"baseline": 31
		},
		{
			"type": "arrow",
			"version": 40,
			"versionNonce": 416691171,
			"isDeleted": false,
			"id": "gaoN0NpZAR0AIWdpsZeO1",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -3749.7218814683642,
			"y": 2353.4446402721337,
			"strokeColor": "#c2255c",
			"backgroundColor": "#fcc2d7",
			"width": 52.26417704887672,
			"height": 200.80798894708823,
			"seed": 1524702574,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693192012325,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "67qkq1ZdJ1JCJJtaW-8-v",
				"gap": 13.226564789919848,
				"focus": 0.0645818129980168
			},
			"endBinding": {
				"elementId": "c8JBO153",
				"gap": 3.666748046875,
				"focus": -0.017552342847873877
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
					52.26417704887672,
					200.80798894708823
				]
			]
		},
		{
			"type": "text",
			"version": 87,
			"versionNonce": 1042611378,
			"isDeleted": false,
			"id": "c8JBO153",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -3921.0563162399617,
			"y": 2557.919377266097,
			"strokeColor": "#c2255c",
			"backgroundColor": "#fcc2d7",
			"width": 469.2602233886719,
			"height": 45,
			"seed": 92523502,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "gaoN0NpZAR0AIWdpsZeO1",
					"type": "arrow"
				}
			],
			"updated": 1693118182841,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "getMovieByCity(movieName)",
			"rawText": "getMovieByCity(movieName)",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "getMovieByCity(movieName)",
			"lineHeight": 1.25,
			"baseline": 31
		},
		{
			"type": "arrow",
			"version": 30,
			"versionNonce": 388327971,
			"isDeleted": false,
			"id": "6mxhrmnFx9rLgCOsn5-q1",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1729.032769406478,
			"y": 3433.8364046831266,
			"strokeColor": "#c2255c",
			"backgroundColor": "#fcc2d7",
			"width": 2.7777099609375,
			"height": 269.44437662760356,
			"seed": 1164950766,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693192012319,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "CcHnRwvvxdoZU5jjTxDNz",
				"gap": 15.06158455413788,
				"focus": 0.042499110704462655
			},
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "triangle",
			"points": [
				[
					0,
					0
				],
				[
					2.7777099609375,
					269.44437662760356
				]
			]
		},
		{
			"type": "text",
			"version": 56,
			"versionNonce": 1423289454,
			"isDeleted": false,
			"id": "XG8XW5HB",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1811.8104793674156,
			"y": 3697.725361388855,
			"strokeColor": "#c2255c",
			"backgroundColor": "#fcc2d7",
			"width": 461.84417724609375,
			"height": 45,
			"seed": 398337710,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1693129041588,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 1,
			"text": "getShows() -> List<shows>",
			"rawText": "getShows() -> List<shows>",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "getShows() -> List<shows>",
			"lineHeight": 1.25,
			"baseline": 31
		}
	],
	"appState": {
		"theme": "dark",
		"viewBackgroundColor": "#ffffff",
		"currentItemStrokeColor": "#c2255c",
		"currentItemBackgroundColor": "#fcc2d7",
		"currentItemFillStyle": "hachure",
		"currentItemStrokeWidth": 1,
		"currentItemStrokeStyle": "solid",
		"currentItemRoughness": 1,
		"currentItemOpacity": 100,
		"currentItemFontFamily": 1,
		"currentItemFontSize": 36,
		"currentItemTextAlign": "left",
		"currentItemStartArrowhead": null,
		"currentItemEndArrowhead": "triangle",
		"scrollX": 4927.618647381849,
		"scrollY": -769.7609223733014,
		"zoom": {
			"value": 0.15000000000000002
		},
		"currentItemRoundness": "sharp",
		"gridSize": null,
		"currentStrokeOptions": null,
		"previousGridSize": null
	},
	"files": {}
}
```
%%