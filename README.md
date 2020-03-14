Hidefy
======

Hidefy is a simple tool for embedding text messages into bitmap images.  
For simplicity, only 24-bit color bitmaps are supported.

<table>
	<tr>
		<th>Before</th>
		<th></th>
		<th>After</th>
	</tr>
	<tr>
		<td><img src="sample.bmp" width="240"></td>
		<td> ⟶  </td>
		<td><img src="sample_stego.bmp" width="240"></td>
	</tr>
</table>

## Motivation

Developed as an excercise and a proof of concept (PoC).

## Building

To compile, simply run:

	$ gcc -Wall -pedantic hidefy.c -o hidefy

## Usage

To encode:

	$ ./hidefy -m "secret message" sample.bmp

To decode: (text is printed to stdout by default)

	$ ./hidefy -x sample_stego.bmp

