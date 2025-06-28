# Docker images

This is a repository of rules used to make docker images. The images should be
built with:

## Building

```bash
docker build -t $USER/image_name:tag image_name/
```

where 
- `$USER` is the dockerhub's user account name.
- `image_name` is the name of the directories.
- `tag` is the name of the version of the image.

E.g:

```bash
docker build -t acampove/rx_run3:v1 rx_run3/
```

## Images

Below is a list of the images and their purpose

### rx_run3

Uses `alma9` CERN image as base, adds HEP software on top
