# Image Locker
A simple python package to encrypt and decrypt images.

## Getting Started
You need to have `python3` and `pip3` in your system.
## about
we also used cryptography, random numbers, hash functions
## Usage
#### encrypt.py
- To get help about the commands `python encrypt.py -h`
  ```
  usage: encrypt.py [-h] [-d DIR] [-f FILE]
  List of commands for Image Encryptor
  optional arguments:
    -h, --help            show this help message and exit
    -d DIR, --dir DIR     The directory path for group of images.
    -f FILE, --file FILE  The path of the file to encrpt.
  ```
- Encrypt a single file `python encrypt.py -f <FILENAME>`
- Encrypt a folder `python encrypt.py -d <FOLDERNAME>`

#### decrypt.py
- To get help about the commands `python decrypt.py -h`
  ```
  usage: decrypt.py [-h] [-d DIR] [-f FILE]
  List of commands for Image Decryptor
  optional arguments:
    -h, --help            show this help message and exit
    -d DIR, --dir DIR     The directory path for group of images.
    -f FILE, --file FILE  The path of the file to encrpt.
  ```
- Encrypt a single file `python decrypt.py -f <FILENAME>`
- Encrypt a folder `python decrypt.py -d <FOLDERNAME>`


##### If the salt file is changed or deleted then the locker won't work so I suggest that create a backup of that file somewhere else.
##### The dimensions of the images without affecting the aspect ratio are reduced to speed up the process. Change the dimensions [here](image_encryptor/__init__.py)

