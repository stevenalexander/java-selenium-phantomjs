# Selenium/PhantomJS web testing container

Docker image with JDK and PhantomJS intended to act as a web testing environment to avoid needing
to install/build web testing tools on your host OS.

NOTE: Building the image takes a long time for PhantomJS compile and I had to increase my Boot2Docker VM memory to 4 gigs to cope.

## Run

Build image:

```
docker build -t stevenalexander/java-selenium-phantomjs .
```

Test PhantomJS:

```
docker run -it --rm phantomjs /phantomjs/bin/phantomjs -v
```
