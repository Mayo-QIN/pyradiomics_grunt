# A RESTFull api for [pyradiomics](https://github.com/Radiomics/pyradiomics)

This is an effort to provide a RESTfull API for pyradiomics utilizing docker and grunt


## Run

clone the repository

```
git clone https://github.com/Mayo-QIN/pyradiomics_grunt.git

```

build docker

```
docker build . -t pyradiomics
```
run docker

```
docker run -d -p 9001:9901 pyradiomics
```

## Usage

visit localhost:9901

  ![image1](/images/1.jpg)

Interact with the service using

- `curl`
```
curl -X POST --form format="txt" --form label="" --form image=@FILENAME --form mask=@FILENAME --form param=@FILENAME --form outputfile=output.FILENAME 0.0.0.0:9001/rest/service/pyradiomics
```

- `python`

- or web interface

  ![image2](/images/2.jpg)
