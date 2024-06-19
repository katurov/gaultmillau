# Gault & Millau, Serbia, jun 2024

I make a map from [Gault &amp; Millau](https://www.gaultmillau.org/?lang=en) in [Serbian cities](https://rs.gaultmillau.com/en/search?keyword=Beograd&lat=45.259199284194004&lng=19.852908236420348&location=all#search)

## How to read

Gault & Millau rates restaurants on a scale of 1 to 20, with 20 being the highest. Restaurants given **below 10 points are rarely listed**. The points are awarded based on the quality of the food, with comments about service, price or the atmosphere of the restaurant given separately. Based on this rating, high-ranking restaurants may **display one to four toques**. Gault Millau does not accept payment for listing restaurants. (c) [Wikipedia](https://en.wikipedia.org/wiki/Gault_Millau#:~:text=6%20External%20links-,Points%20system,of%20the%20restaurant%20given%20separately.)

## WHY

It isn't easy to understand which restaurant is near to you, your hotel, your route without map representation. So I made different formats of the map, depending of the application you use for navigation. Here are main files and formats. If you know more about them, lets discuss it in "Issues".

## How to use 

Easiest way: just look at [this Google Map](https://www.google.com/maps/d/edit?mid=1Mwi2caXIcMzMn9bvnTP8SXFbp25bK7c&usp=sharing) for Novi Sad and Belgrade (in English) or [this one](https://www.google.com/maps/d/edit?mid=11Ptmsc-cIpG8_q-QB756v31Nzp1Glhc&usp=sharing) for whole Serbia (is Serbian).

Hard way: download file and put into your desired application

## Files
| File | City | Format | Where to use |
| ---- | ---- | ------ | ------------ |
| Gault & Millau in Serbia.gpkg | Serbia | GPKG | QGIS |
| Gault & Millau in Serbia - Google (SRB).kml | Serbia | KML with HTML | Google Maps |
| [Gault & Millau in Serbia (SRB).kml](https://raw.githubusercontent.com/katurov/gaultmillau/main/Gault%20%26%20Millau%20in%20Serbia%20(SRB).kml) | Serbia | KML | [Organic Maps](https://github.com/organicmaps/organicmaps) |
| Gault & Millau in Beograd.gpkg | Belgrade | GPKG | QGIS |
| Gault & Millau in Beograd - Google.kml | Belgrade | KML with HTML | Google Maps |
| [Gault & Millau in Beograd - OSM.kml](https://github.com/katurov/gaultmillau/blob/main/Gault%20%26%20Millau%20in%20Beograd%20-%20OSM.kml) | Belgrade | KML | [Organic Maps](https://github.com/organicmaps/organicmaps) |
| Gault & Millau in NoviSad.gpkg| Novi Sad | GPKG | QGIS |
| Gault & Millau in Novi Sad - Google.kml | Novi Sad | KML with HTML | Google Maps |
| [Gault & Millau in Novi Sad - OSM.kml](https://github.com/katurov/gaultmillau/blob/main/Gault%20%26%20Millau%20in%20Novi%20Sad%20-%20OSM.kml) | Novi Sad | KML | [Organic Maps](https://github.com/organicmaps/organicmaps) |

To open in Organic Map or ANY suitable for KML format from mobile just click on the file name.

## Top 5 levels in Serbia
| Level | Title | Score | Toques |
| ----- | ----- | ----- | ------ |
| _1_ | [FLEUR DE SEL](https://sapat.rs) | 17.5 | 4 |
| _2_ | [SALON 1905](https://www.salon1905.rs/) | 17.0 | 4 |
| _2_ | [LANGOUSTE](https://www.langouste.rs/) | 17.0 | 4 |
| _3_ | [LA PISTA](https://www.gorskihotel.com/gorski/la-pista-restoran) | 16.0 | 3 |
| _3_ | [THE SQUARE](https://squarenine.rs/) | 16.0 | 3 |
| _4_ | [RESTORAN 27](https://restoran27.rs) | 15.5 | 3 |
| _4_ | [RESTORAN GIG](https://restorangig.rs/) | 15.5 | 3 |
| _5_ | [JAM - JUST A MAESTRO](https://www.justamaestro.rs/) | 15.0 | 3 |
| _5_ | [PROJECT 72 WINE&DELI](https://project72.rs/) | 15.0 | 3 |
| _5_ | [HOMA](http://www.homa.rs/) | 15.0 | 3 |
| _5_ | [ENSO](https://www.enso.rs) | 15.0 | 3 |

## Top in Novi Sad
| Title | Score | Toques |
| ----- | ----- | ------ |
| [PROJECT 72 WINE&DELI](https://project72.rs/) | 15.0 | 3 |
| [FISH&ZELENIŠ](https://www.fishizelenis.com/) | 14.5 | 2 |
| [JASMIN A MASLINA](https://www.instagram.com/jasmin_a_maslina/) | 14.0 | 2 |
| [LE KLOK BISTRO](https://www.instagram.com/le_klok_bistro/) | 13.5 | 2 |
| [KONOBA RIBA RIBI GRIZE REP](https://www.rrgr.rs/) | 13.5 | 2 |
| [CUBO](http://www.cubonovisad.rs) | 13.0 | 2 |
| [PETRUS](https://petruscaffe.com/) | 12.5 | 1 |
| [SOKAČE](https://www.sokace.rs/) | 12.0 | 1 |
| [PIKNIK](https://piknik.rs/) | 12.0 | 1 |
| [RESTORAN VELIKI](https://cafeveliki.com) | 12.0 | 1 |
| [KORPA DELI MARKET I BISTRO](https://korpa-deli.rs) | 12.0 | 1 |
| [SAVOCA](https://savocapicerija.rs) | 11.5 | 1 |
| [RESTORAN KOD BRKE](https://kodbrke.rs/) | 11.0 | 1 |

# The process

1. Read data from G&M website
2. Use OSM to get coordinates for addresses (we will have a lot)
3. Save "dirty" JSON for backup
4. Use data to generate GPKG file and transform in into KML for Google
5. Check on Google are all poins on their places
6. Corect some (delete, move)
7. Check that all poins from original file found on map
8. Correct some
9. Creade GPKG file (two versions: plain text and HTML-able)
10. Upload to suitable app to check

# Read Next

[The map of Michelin in Belgrade](https://www.google.com/maps/d/edit?mid=1XRS97kY_y-CPb49jsHTl5hwT_ey_C94&usp=sharing) as part of my "[where to eat and drink](https://docs.google.com/spreadsheets/d/1t_3RsxL-eRH5kTqMl_QjdIJJrjZJaE6oCikJun-_h7U/edit?usp=sharing)" project.

[Really cool](https://www.facebook.com/nepusackilokaliubeogradu/) group on Facebook for years supports a [Map of non-smoking restaurants and caffee in Belgrade](https://www.google.com/maps/d/viewer?mid=1qkPRUNRiCqA-uFugbcuVy9INXgw&shorturl=1&ll=44.81601345502995%2C20.4492096243896&z=12). Wish someone will make a global Map.
