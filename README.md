# Scala and sbt Dockerfile

[Scala](http://www.scala-lang.org) and [sbt](http://www.scala-sbt.org) container.

Useful for building in environments like CircleCI v2.


## Base Docker Image ##

* [openjdk:8-jre-alpine](https://hub.docker.com/_/openjdk)


## Installation ##

1. Install [Docker](https://www.docker.com)
2. Pull [automated build](https://hub.docker.com/r/spikerlabs/scala-sbt/) from public [Docker Hub Registry](https://hub.docker.com):
3. See [tags](https://hub.docker.com/r/spikerlabs/scala-sbt/tags/) for built specific versions (not the latest ones)
```
docker pull spikerlabs/scala-sbt
```
Alternatively, you can build an image from Dockerfile:
```
docker build -t scala-sbt github.com/spikerlabs/scala-sbt
```
Or with specific versions:
```
docker build -t scala-sbt --build-arg SCALA_VERSION=2.12.7 --build-arg SBT_VERSION=1.2.6 github.com/spikerlabs/scala-sbt
```

## Usage ##

```
docker run -it --rm spikerlabs/scala-sbt /bin/bash
```


## Contribution policy ##

Contributions via GitHub pull requests are gladly accepted from their original author. Along with any pull requests, please state that the contribution is your original work and that you license the work to the project under the project's open source license. Whether or not you state this explicitly, by submitting any copyrighted material via pull request, email, or other means you agree to license the material under the project's open source license and warrant that you have the legal authority to do so.


## License ##

This code is open source software licensed under the [Apache 2.0 License](http://www.apache.org/licenses/LICENSE-2.0.html).

This is forked repository with optimisations on top of original [hseeberger/scala-sbt](https://github.com/hseeberger/scala-sbt).
