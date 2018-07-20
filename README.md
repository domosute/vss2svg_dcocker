# vss2svg_docker
Dockerfile for an excellent Visio Stencil converter created by [kawka].(https://github.com/kakwa/libvisio2svg)

## How to build and run
1. Pull this repo.
```
$ git clone https://github/domoste/vss2svg_docker.git
```
2. Build
```
$ cd vss2svg_docker
$ docker build -t vss2svg .
```
3. Run
```
$ docker -dit --name vss2svg -v $PWD:/opt vss2svg bash
```
4. Exectute in the docker container, download visio stencil and convert vss file with vss2svg-conv.
```
$ docker exec -it vss2svg bash
```

## How to Convert Visio Stencil
```
$ vss2svg-conv -i <input>.vss -o <output directory>
```

