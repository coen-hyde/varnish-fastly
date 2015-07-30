Varnish 2.1.5
=============

This is an old version of Varnish (same version Fastly uses).

Usage
-----

```
docker run -d \
  -v $PWD:/data \
  --env 'VCL_CONFIG=/data/varnish.vcl' \
  coenhyde/varnish-fastly
```

The VCL_CONFIG must point to your varnish config. Mount a volume and point
VCL_CONFIG to the vcl file in the mount.
