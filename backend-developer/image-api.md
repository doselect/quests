# Image Management API

The world as we know it is going nuts over sharing images. The total number of
images our civilization is producing, hence, is growing exponentially every
year. People who build applications that use images need to be extra smart
when it comes to managing those images.

You need to solve this problem with a REST API.


## Description

Create a service which exposes a RESTful API, that can be used to manage
images used by other services. This service can be used to store, update,
retrieve and delete images.

Keep in mind the following points. These are required:
 - The image should be stored on the file-system where this service lives.
 - To use this API, an API access key has to be generate using a management
 command. This access key should be used to authenticate all API calls.
 - You MUST NOT use any database to store image metadata. A filesystem where you
 store the images is all you have.

Good to haves:
 - Lossless compression of images
 - Support for more image types (PNG, JPEG, GIF)
 - Endpoint to re-generate the access key 


## API specs

The following URL patterns should be mapped with various functionalities of the
API:

 - **GET** list: all images linked to the provided access key
 - **GET** detail: one image
 - **POST** list: create a new image
 - **PATCH** detail: update one image
 - **DELETE** detail: delete one image


## Technologies

You are free to use any programming language / framework for building this
service. However, if you have applied for a technology specific position, it
would be great to use the same.
