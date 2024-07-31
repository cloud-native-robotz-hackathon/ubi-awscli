# ubi-awscli
[![Docker Repository on Quay](https://quay.io/repository/cloud-native-robotz-hackathon/ubi-awscli/status "Docker Repository on Quay")](https://quay.io/repository/cloud-native-robotz-hackathon/ubi-awscli)

Unofficial image for AWS CLI based on Red Hat Universal Base Image v9

## Why another image?

This image was build using the [Red Hat Universal Base Image (UBI) 9](https://developers.redhat.com/products/rhel/ubi/), which provides a stable foundation to workloads running on mission-critical environments, specially on **Red Hat OpenShift Container Platform**.

## How to use?

If you running standalone containers, you can use `podman` or `docker` with:

```bash
export IMAGE='quay.io/cloud-native-robotz-hackathon/ubi-awscli:1.25.83'
podman build --platform linux/amd64,linux/arm64  --manifest ${IMAGE}  .
podman manifest push ${IMAGE}
```

## Any support?

This is a community project, not backed nor supported by Red Hat.
