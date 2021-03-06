.. imageprocess_server documentation master file, created by
   sphinx-quickstart on Wed May  2 18:25:12 2018.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to imageprocess_server's documentation!
===============================================

.. toctree::
   :maxdepth: 2
   :caption: Contents:

"""
    app_get_user Function takes the user_email input from the user, which
    help user to get his own images data from database with all the images
    information.

    :param email: str of the user email

"""

"""
    Remove the header of the images base64 bytes from front-end
    :param image_str: the input should be the base64 bytes of the image

    :returns: base64 string without data header

    :rtype: string

"""

"""
    After the specific image processing, this function process all the
    information regarding this image. After processing, this would return a
    image array including the corresponding information of the image,
    including: base64 str of the images, filename, id, process type, time
    stamp, time duration and processed histograms.
    :param filename: str of the name of the image
    :param protype: list of the post-processed image histogram
    :param proc_cmd: the str of process command which would be Reverse Video,
    Contrast Stretching, Log Compression and Histogram Equalization.

    :returns: a python array contains all the information fo the image after
    processing, including base64 str of the processed images, filename, id,
    process type, time stamp, time duration and processed histograms.

    :rtype: an array with string value

"""

"""
    create_user Function takes the user_email input from the user including
    their setting email and their names. This function store and establish
    the user profile in the database.
    :param email: str of the user email
    :param name: str of the user name

"""


"""
    Remove the header of the images base64 string from front-end
    :param images: the input should be the base64 string of the image
    :raises TypeError: if input is not a string

    :returns: base64 string without data header

    :rtype: string

"""

"""
    images_post Function takes the input from the user such as email, images
    and the image filename, which performs the desired pre-processing on the
    image and saves as an array containing image information to the database.

    :param email: str of the user email
    :param images: base64 string of the images with headers from front-end
    :param filename: the str of images name as its specific identification

"""

"""
    pro_images_post Function takes the input from the user such as email,
    images the image filename as identification and process type command,
    which performs the desired processing procedure on the image and saves
    as an array containing image information to the database.

    :param email: str of the user email
    :param process: process types of command
    :param images: base64 string of the images with headers from front-end
    :param filename: the str of images name as its specific identification

"""


"""
    This MongoModel store the data into database.
    :param email: EmailField to store user emails
    :param name: CharField to store user names
    :param images: ListField to store original images
    with their information including the base64 str of the images,
    filename, id, filetype, time stamp, image size and unaltered
    histograms.
    :param pro_images: ListField to store processed images
    with their information including base64 str of the images, filename,
    id, process type, time stamp, time duration and processed histograms.

"""

"""
    Appends images to specific user email and the images corresponding
    information, including the base64 str of the images, filename, id,
    filetype, time stamp, image size and unaltered histograms.
    :param email: str email of the user
    :param image_info: a list of image information

"""

"""
    After processing, this function is to appends images to specific user
    email and the images corresponding information, including the
    base64 str of the processed images, filename, id, process type,
    time stamp, time duration and processed histograms.
    :param email: str email of the user
    :param image_info: a list of image information

"""

"""
    Creates a user with the specified email and name. If the user already
    exists in the DB this will overwrite that user.
    :param email: str email of the new user
    :param name: str name of the new user

"""

"""
    Check if the user exists in the database. If user exists, this will
    return > 0, if not it would be 0.
    :param email: str email of the new user

"""

"""
    Prints the user with the specified email
    :param email: str email of the user of interest
    :return:

"""



Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
