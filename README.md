# shp2leaflet
A geeky testbed for loading .shp files client-side using Leaflet + shp.js. “Let me quickly check this layer”

**Viewr**  
![image](img/viewr.gif)

#### Running Locally

I used Shapefile archives compressed as `.zip`, which needed to be loaded via a local web server in the same folder as the HTML file to work properly.

I used Python's built-in HTTP server for this. This server makes the files accessible via HTTP, which avoids security restrictions that occur when opening files locally with file://.

```shell
# Navegue até o diretório onde estão os arquivos .shp

cd C:\Users\JesseBurlamaque\Documents\GitHubProjects\shp2leaflet

python -m http.server 8000
```

#### In the browser

After starting the server, in web browser:

http://localhost:8000
