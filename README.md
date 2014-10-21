# Ubuntu LTS is FISMA-ready

This project creates hardened, FISMA-compliant Ubuntu LTS AMIs that are suitable for use in the Amazon Web Services public cloud.

(It may expand soon to support other deployment environments and image types.)

Prepared and maintained by **[18F](https://18f.gsa.gov)**, a technology team inside the US federal government.

## Setup

* Install [Packer for your OS](http://www.packer.io/downloads.html). At press time, we used Packer 0.7.1.

```bash
$ packer -v
Packer v0.7.1
```

* Set two environmental variables.

```bash
export AWS_ACCESS_KEY_ID=[your AWS access key]
export AWS_SECRET_ACCESS_KEY=[your AWS secret key]
```

## Building the AMI

1. Run `ami.sh`.

That's it! Take note of the AMI ID this spits out to your console after it's done.
