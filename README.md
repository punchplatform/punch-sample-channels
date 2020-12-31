# punch-sample-channels

This repository provides a number of sample channel
that illustrate what you can do with the punch. 

Note that the punch documentation provides more advanced referenced configuration
that are used in production systems. Here we provide simpler yet illustrative examples
that may be useful for you to explore the many punch configuration possibilities. 

Checkout the README.md file in each repository. 

The sample channels provided here are grouped as part of a 'sample' tenant. That makes it easy to
install these sample on your standalone or production platform. 

To install on you standalone, simply copy or link these channels as part of one of 
your tenant. The simplest is to just type in

```sh
ln -s samples $PUNCHPLATFORM_CONF_DIR/tenants/samples
```
From there you can start the channels using the interactive punch cli
```sh
channelctl --tenant samples
```
