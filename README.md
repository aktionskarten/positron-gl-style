# Positron

A Mapbox GL basemap style useful for data visualizations. The cartography is based on the
[CartoDB Positron Basemap](https://github.com/CartoDB/CartoDB-basemaps) and it is using the vector tile
schema of [OpenMapTiles](https://github.com/openmaptiles/openmaptiles).

## Edit the Style

Use the [Maputnik CLI](http://openmaptiles.org/docs/style/maputnik/) to edit and develop the style.
After you've started Maputnik open the editor on `localhost:8000`.

```
maputnik --watch --file style.json
```

## Sprites Generation

The `dolomate/spritezero` docker image was used for sprite generation:

```
docker run -it -e FOLDER=_svg -e THEME=sprites -v ${PWD}/data:/data dolomate/spritezero
```

as described in [https://github.com/macteo/spritezero-docker](https://github.com/macteo/spritezero-docker)
