
<p align="center">
<img src="http://www.itowns.fr/images/logo-itowns2XS.png" />
</p>

# iTowns V1

### What is it?

iTowns is a web framework written in Javascript/WebGL for visualisation of 3D geographic data allowing precise measurements in 3D.
Its first purpose was the visualisation of street view images and terrestrial lidar point cloud. It has then been extended to handle more data types.

### Supported data types

- Oriented images
- Panoramic images
- Point Clouds
- 3D textured models
- WFS Vector
    
![iTowns screenshot](http://www.itowns.fr/videos/screenshotGIT.jpg)

The V1 of iTowns Open Source is the core of the original iTowns from IGN Matis lab. As such, it contains a subset of the original application features.

### Features

- Load and project Oriented Images on mesh (cube or city model)
- Load and display Panoramic Images
- Load Depth Panoramic Image and render in 3D
- Load 2D multipolygons with height (building footprint) from WFS or local file and triangulate it to create building boxes. This mesh can then be use for texture projection.
- Navigate through Image Data using click and go functions
- Load and display Point Cloud from PLY files.
- Load and display 3D textured models (B3D, 3DS).
- Simple API interface.

### Sample data

You can test iTowns with a provided sample data set, courtesy of French IGN.

The sample data is here : https://github.com/iTowns/itowns-sample-data

It includes :

- 250 Oriented Images (50 Panoramics, 192 MB)
- 1 patch (500 * 500m) of 3D textured city models (BATI3D, 50 MB)
- Terrestrial PointCloud (20 Millions point, 400 MB)
- JSON of building footprint and DTM (500 kB)

### Getting started

You have to clone the iTowns and sample data repositories, start a webserver, and you have a running demo.

Open a command line and run :

```
git clone https://github.com/iTowns/itowns.git itowns
git clone https://github.com/iTowns/itowns-sample-data.git
cd itowns
ln -s ../itowns-sample-data ./data
python -m SimpleHTTPServer
```

Now open [http://localhost:8000](http://localhost:8000) and enjoy !

### Notes

The application should be able to work without the need of a local database or PHP scripts. But you will still need to have a local server running like apache.

### Roadmap items

The following tasks are currently worked on :

- Code simplification
- Documentation
- Offline examples
- Python code for data preparation

Meanwhile, iTowns version 2 is also at the design phase.

### Support

iTowns is an original work from French IGN, MATIS research laboratory.
It has been funded through various research programs involving the French National Research Agency, Cap Digital, UPMC, Mines ParisTec, CNRS, LCPC.

iTowns is currently maintained by IGN ( http://www.ign.fr ) and Oslandia ( http://www.oslandia.com )

![IGN Logo](https://raw.githubusercontent.com/iTowns/itowns/master/images/IGN_logo_2012.png)
![Oslandia Logo](https://raw.githubusercontent.com/iTowns/itowns/master/images/Oslandia_logo.png)
