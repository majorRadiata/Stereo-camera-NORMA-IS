# Stereo-camera-NORMA-IS
A small part of main development of machine vision stereo setup at Norma IS, Saint-Petersburg, RU.

calibration.hdev contains script for calibrating stereo camera to get the real world coordinates on images. Input data: a set of calibration plate images from each camera, internal camera parameters (size of pixel, focus, image width, image height), calibration plate parameters. Output: returns parameters of calibration and a calibration error, it corresponds to the average distance (in pixels) between the backprojected calibration points and their extracted image coordinates.

stereosearch.hdev contains script for reconstruction of surfaces (cloud of 3d points) and searching the desired object in it. Input data: a 3d model of object, internal parameters of cameras, calibration parameters, images of the object from cameras. Output: 3d recostruction of surface (cloud of 3d point), the real world coordinates of the object.
