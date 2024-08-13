<html>
    <head>
        <title>Rent Affordability in San Francisco, 2013</title>
        <meta charset="utf-8"/>
        <link rel="stylesheet" href="https://unpkg.com/maplibre-gl@3.3.1/dist/maplibre-gl.css" crossorigin="anonymous">
        <script src="https://unpkg.com/maplibre-gl@3.3.1/dist/maplibre-gl.js" crossorigin="anonymous"></script>
        <script src="https://unpkg.com/pmtiles@3.0.5/dist/pmtiles.js"></script>
        <style>
            body {
                margin: 0;
            }
            #map {
                height:100%; width:100%;
            }
        </style>
    </head>
    <body>
        <div id="map"></div>
        <script type="text/javascript">

            let hoveredStateId = null;

            // add the PMTiles plugin to the maplibregl global.
            let protocol = new pmtiles.Protocol();
            maplibregl.addProtocol("pmtiles",protocol.tile);

            let PMTILES_URL = "https://mizmay.github.io/RentAffordability/RentAffordability-OneBr.pmtiles";

            const p = new pmtiles.PMTiles(PMTILES_URL);

            // this is so we share one instance across the JS code and the map renderer
            protocol.add(p);

            // we first fetch the header so we can get the center lon, lat of the map.
            p.getHeader().then(h => {
                const map = new maplibregl.Map({
                    container: 'map',
                    zoom: h.minZoom,
                    center: [h.centerLon, h.centerLat],
                    style: {
                        version:8,
                        sources: {
                            "sf_rent": {
                                type: "raster",
                                url: "pmtiles://" + PMTILES_URL,
                                attribution: '© Stephanie May',
                                tileSize: 256
                            }
                        },
                        layers: [
                            {
                                "id": "raster-tiles",
                                "type": "raster",
                                "source": "rent_sf",
                            }
                        ]
                    }
                });
            });
        </script>
    </body>
</html>