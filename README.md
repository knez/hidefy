Hidefy
======

Hidefy is a simple tool for embedding text messages into bitmap images.  
For simplicity, only 24-bit color bitmaps are supported.

## Motivation

Developed as an excercise and a proof of concept (PoC).

## Building

To compile, simply run:

	$ gcc -Wall -pedantic hidefy.c -o hidefy

## Usage

To encode:

	$ ./hidefy -m "secret message" cover_image.bmp

To decode: (text is printed to stdout by default)

	$ ./hidefy -x stego_image.bmp

