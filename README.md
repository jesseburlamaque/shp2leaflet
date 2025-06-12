# shp2leaflet

[![Leaflet](https://img.shields.io/badge/Leaflet-199900?logo=leaflet&logoColor=white)](https://leafletjs.com/)
[![React](https://img.shields.io/badge/React-20232A?logo=react&logoColor=61DAFB)](https://reactjs.org/)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![Netlify](https://img.shields.io/badge/Netlify-Live-00C7B7?logo=netlify&logoColor=white)](https://shp2leaflet.netlify.app/)
![GIS](https://img.shields.io/badge/GIS-Shapefile%20Viewer-blue)

A geeky testbed for loading .shp files client-side using Leaflet + shp.js. “Let me quickly check this layer”

**Viewr**  
![image](img/viewr.gif)

#### Running Locally

I used Shapefile archives compressed as `.zip`, which needed to be loaded via a local web server in the same folder as the HTML file to work properly.

I used Python's built-in HTTP server for this. This server makes the files accessible via HTTP, which avoids security restrictions that occur when opening files locally with file://.

```shell
# directory where the .shp files are located

cd C:\Users\JesseBurlamaque\Documents\GitHubProjects\shp2leaflet

python -m http.server 8000
```

##### In the browser

After starting the server, in web browser:

http://localhost:8000

#### Hosting Online

This project is available online via:

- **GitHub Pages:** [https://jesseburlamaque.github.io/shp2leaflet/](https://jesseburlamaque.github.io/shp2leaflet/)
- **Netlify:** [https://shp2leaflet.netlify.app/](https://shp2leaflet.netlify.app/)

#### Latency & Hosting Benchmark

What started as a simple file viewer turned into an interesting experiment in comparing latency across different hosting platforms.

This app is now being used to test response time for lightweight assets hosted on:

- GitHub Pages
- Netlify

Early results focus on minimal apps, but upcoming tests will involve larger webapps to evaluate how performance scales with size and complexity.

**Notebook Jupyter:** [latency_benckmark_app_v2.ipynb](https://github.com/jesseburlamaque/shp2leaflet/blob/main/latency_benckmark_app_v2.ipynb)


**Figure 1 - Total Time to First Byte**  
![image](img/v1-time-to-first-byte.png)

**Figure 2 - Total Time Response**  
![image](img/v1-total-time-response.png)

**Figure 3 - Download Time**  
![image](img/v1-download-time.png)

