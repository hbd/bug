# Bug - Braille Unicode Graphics

Use braille pixelation to render images in the termincal.

## Features

0 dependencies: everything in `bug` is only useing the stdlib, including the tests.

Importing `bug` will register the format on the `image` stdlib package, allowing for the use of `image.Decode`.

As `bug` implements the `image.Image` interface, it can be use like any other image types.

## File types

The expected file type when storing images on disk is `.bug`.

## Limitations and Future improvments

It would be intersting to try to add support for colors. We could only have one color per 2x4 pixel block, but I'd be currious to see how it looks like.

While `bug` will work with any image, it will render best with black and white images.

## Unicode Patterns

https://en.wikipedia.org/wiki/Braille_Patterns#Block

## Examples

From [Golang's website](https://golang.org/doc/gopher/) under [Creative Commons Attribution 3.0 License](Creative Commons Attribution 3.0 License).

```
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣀⣀⣢⣤⣤⣤⣵⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣐⣠⣵⡾⠿⡛⠛⠩⠁⠀⠀⠈⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⡀⣢⣤⣶⠿⠟⠫⠅⠘⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⡀⣠⣾⢟⠉⠒⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⢖⣤⡾⠫⠔⠁⠀⠀⠀⠀⡀⠀⣀⣠⣤⣭⣥⣤⣤⣤⣤⣀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣀⡀⠀⢀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠸⠟⠫⠂⠀⠀⢀⠠⣫⣥⣴⡾⠿⠛⠋⠉⠉⠁⠀⠂⠉⠩⠙⡻⢶⣅⠤⡀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣠⣥⣶⣶⠿⠿⠿⠿⠿⠿⠿⠿⣷⣮⣁⢄⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣵⠾⠫⠩⠷⠀⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠁⠐⠙⠳⣦⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⡀⣚⣤⣾⠟⠛⠉⠁⠂⠁⠁⠀⠀⠀⠀⠉⠁⠐⠉⡻⢷⣌⡠⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠋⠑⠉⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠁⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⡠⣪⣾⠟⠉⠂⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠐⢙⠻⣮⡠⢀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢄⣀⠄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣽⣿⢱⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠉⠊⠻⣷⣄⢀⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣀⠀⣠⣿⣹⣧⣂⣀⠄⢀⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣿⣿⣦⠆⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠉⠊⠿⣷⣕⢤⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⡀⢀⣵⡾⢟⠛⠛⠛⠋⢙⠻⢶⣥⣂⢤⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠙⣷⡻⣧⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠊⡻⣷⣅⢢⡀⠀⠀⠀⠀⢀⢐⣢⣤⣤⣵⡟⡉⠈⠀⠀⠀⠀⠀⠀⠈⠁⠈⠛⢷⣕⠢⠤⠠⢀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠤⣀⣀⡀⠄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠚⢷⣜⢿⣦⣠⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠨⣝⢷⣦⡠⡀⠀⠀⣰⣿⠿⣶⣌⡻⣿⣄⠄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠰⣻⣿⠿⠿⣷⡅⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠠⣐⣴⣾⠿⠿⠛⠿⢿⣮⡀⠄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠻⣷⡝⢷⣔⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠑⠝⠿⣮⡃⢳⣿⣥⡂⢸⣿⠈⠨⢛⠿⣶⣤⣄⡠⡀⠀⠀⠀⠀⠀⠀⠙⣿⣿⢇⣿⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢠⢄⣵⣾⠟⠫⠀⠀⠀⠀⠀⠱⢝⢿⣯⡢⡄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠰⡽⣿⣦⡙⢿⣄⠢⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⡻⣿⣿⡿⠃⣼⣏⠄⢀⣤⣶⣶⣮⣝⢿⣮⡂⠀⠀⠀⠀⠀⠀⣿⣷⣿⢟⠀⠀⠀⠀⢀⢀⣀⣤⣔⣀⠀⠀⠀⠀⠀⠀⠀⠰⣵⣿⢟⠄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠱⠻⣿⡆⡄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠸⠹⣿⢷⣥⡙⢿⣬⠆⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⢨⢿⣿⣿⣿⡿⣷⣿⡟⠁⡀⠍⢻⣧⠹⣷⡰⠀⠀⠀⠀⠀⢅⣠⣿⠀⠀⠀⠀⠀⣳⡿⢛⡉⣙⢛⠿⣶⣥⡂⠀⠀⠰⣼⡿⡱⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢻⣿⡄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⡀⢀⣻⣯⣿⣿⣦⣙⢿⣮⡂⣀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢘⣿⣿⠙⠿⣿⣿⡿⣿⠆⠀⢸⣿⠀⣿⢷⣦⣤⣴⣶⡶⠟⣫⣿⠀⠀⢀⢔⣵⣿⣿⣿⢿⣧⠀⠁⠂⢙⢿⣷⣤⣼⡿⡅⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣿⣧⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠰⣥⣶⡾⠿⠛⢻⣾⣿⠻⣷⣄⠝⠿⣦⡑⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⣿⢻⣷⣦⣼⡿⣷⣄⣒⣨⣾⠏⣼⣿⣤⣀⣀⣀⣠⣴⣾⣿⡏⠀⠀⣰⡿⣋⣴⣾⣿⣿⠏⠆⠀⠀⠀⠓⢸⣿⡿⡅⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢹⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⣿⣧⡂⠀⠀⠀⡻⣿⢯⠢⠝⢷⣄⡨⡻⣦⡕⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣾⣿⠿⣷⣟⣛⢿⣮⣛⡛⣛⣡⣾⠟⡭⠛⣿⡟⠛⠛⠍⠀⣿⢇⠰⣵⣿⣽⡟⡩⠂⠹⣿⣦⣢⡀⠀⠀⢀⣾⠟⠜⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⣷⡹⣿⣄⢄⡀⠘⠂⠀⠀⠀⠐⠙⢿⣮⡪⡻⣦⡕⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣿⡇⠀⠐⠋⠀⠓⠉⠛⠿⠿⠛⠥⠃⠀⠈⢸⣷⠀⠀⠀⠸⣿⣴⡾⢋⣾⢟⠆⠀⠀⠀⠈⢻⣷⣬⡣⢄⣾⠏⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣾⡟⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠹⣷⣌⠻⣷⣅⠀⠀⠀⠀⠀⠀⠀⠐⢝⢿⣮⡪⡻⣮⡃⣀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢿⣇⠄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣿⡄⠄⠀⠘⠉⢁⣤⣾⢯⠎⠀⠀⠀⡀⠀⠐⢝⣿⣿⣿⡏⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣿⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠪⠛⣷⣌⠻⣷⣔⢄⠀⠀⠀⠀⠀⠀⠑⠝⢿⣦⡨⡻⣮⡣⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢘⢿⣦⢄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠛⠿⢷⣿⣿⠟⠋⣂⣡⣬⣭⣤⣶⣾⣿⠿⠿⢛⣿⡟⢀⠀⠀⠀⠀⣀⣀⣀⣀⣀⣀⣀⣀⣀⣀⡀⠀⠀⠀⠀⢀⣿⠃⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠀⠙⢷⣌⠙⢷⣅⢄⠀⠀⠀⠀⠀⠀⠀⢝⢿⣦⡘⠿⣮⡀⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠈⠻⣷⣄⡠⠀⡀⡷⣦⣶⣤⣀⠀⠀⠀⣀⡀⠀⠈⠀⣾⡿⠿⠿⠛⠛⠉⠉⠑⠀⠀⠀⠈⠁⣼⣿⣷⣶⣶⡾⠿⠿⠟⠛⠛⠛⠉⠉⠉⠙⠛⠛⠻⣷⣄⢀⠀⣸⡿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠑⢙⢷⣤⡙⢷⣜⠄⠀⠀⠀⠀⠀⠀⠁⣿⢿⣮⡙⢿⣭⡂⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠀⠙⠻⠷⣶⣶⣿⣥⣾⣯⣶⣶⣶⣶⣶⣶⣄⣠⣿⠃⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠉⠐⠒⠀⠀⠀⣣⣶⡿⠟⠿⠿⠿⠿⠿⠟⠛⠛⠛⠻⢿⣷⣴⡿⡓⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠑⣝⢿⣮⡻⢷⣄⠢⡄⠀⣀⠀⣀⣼⣿⣿⣿⣦⡙⢿⣤⡢⣀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠁⠀⠀⠈⠉⠉⠉⠁⠀⠀⠀⠊⢙⠻⣿⣏⢇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⡻⣯⣿⣦⡢⠀⠀⠀⠀⠀⠀⠀⠀⠀⠁⠪⠻⣷⣄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠐⣝⢷⣌⠻⣷⣄⣢⣴⡿⢟⠋⠑⠀⠊⡻⢷⣅⡙⢿⣮⡢⢀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⢪⡻⣷⣄⢄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠊⡻⣮⣻⣮⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠘⢊⢿⣦⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⣠⣶⣦⣒⢀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠁⢙⢿⣾⣿⠟⡫⠂⠀⠀⠀⠀⠀⠈⠐⠙⢷⣆⢝⠻⣮⡢⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢮⠻⣷⣄⢤⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠪⠻⣿⣿⣦⣐⠄⠀⠀⠀⠀⠀⠀⠀⠀⠐⠹⣿⣄⠄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⣿⡏⠍⢿⣮⢦⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢠⡿⠋⠅⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠪⡻⣷⣕⢉⠻⣮⣀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠊⡻⣷⣕⢤⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠨⢙⢿⣝⢷⣅⣠⠀⠀⠀⠀⠀⠀⠀⠀⠎⢿⣦⣢⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⢻⣇⠀⠀⢻⣧⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣽⢟⠅⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠠⣝⢷⣍⠪⡻⣷⣕⠄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠎⠻⣷⣅⠄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠝⣷⣿⡷⣥⡢⠀⠀⠀⠀⠀⠀⠀⠰⢻⣷⣠⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠰⣤⡞⣿⡄⠀⠰⢻⣧⠆⠀⠀⠀⠀⠀⠀⣞⣼⠏⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠁⢙⢷⣍⠈⡻⣷⣅⢤⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠎⡻⣷⣔⢄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⢀⣾⠟⠉⠻⣾⣿⣶⣕⠠⡄⠀⠀⠀⠀⠀⢻⣷⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠰⣼⠏⣃⡘⣿⡄⠀⢠⢿⣇⠀⠀⠀⠀⠀⠘⣾⠿⠿⣷⣕⠂⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠐⠝⢷⣝⠮⡻⣷⣅⠄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠁⠨⠻⣷⣐⢆⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⠀⣢⣴⢟⡫⠂⠀⠀⠐⠝⠻⣿⣿⣦⣄⣂⠀⠀⣒⣼⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⢰⡟⢰⡟⠁⠹⣿⡴⡀⠞⣿⡀⠀⠀⠀⠀⣸⣯⠀⠀⠂⠛⢿⣜⠆⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠓⢝⢷⣮⡨⡻⣷⣝⠀⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠨⡻⣷⣕⢀⠀⠀⠀⠀⠀⡀⢖⣵⡾⠫⠑⠃⠀⠀⠀⠀⠀⠀⠀⠂⠝⠛⠿⣿⣿⡿⠿⡛⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⣿⠁⣿⠁⠀⠀⠹⣿⡝⡼⢹⣧⠀⠀⠀⢸⡿⠀⠀⠀⠀⠀⠣⡻⣧⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠳⡽⣿⣆⠪⣝⢷⣬⡢⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠘⠮⡻⣷⣕⢄⢀⢐⣨⣾⢟⠉⠂⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠒⠐⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⣿⢰⣿⠀⠀⠀⠀⠙⣿⣞⢃⣿⡄⠀⠀⣿⠇⠀⢀⠀⠀⠀⠀⠀⢹⣇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠘⠪⠻⣷⣄⠓⣝⢷⣮⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠘⢪⡻⣷⣶⡿⠛⠁⠃⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⣿⢸⡇⠀⠀⠀⠀⠀⢘⢿⣎⢸⣧⠀⢰⣿⠿⠿⣶⣅⢄⠀⠀⠀⠀⢿⡄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠊⠻⣷⣮⠳⡙⢷⣄⢀⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠁⠈⡻⣷⣕⢄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⣿⢸⣇⡄⠀⠀⠀⠀⠀⠫⢻⣯⣿⣆⣿⠣⡋⠀⠀⠙⣷⡁⠀⠀⠀⢸⣷⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⢌⣿⣿⣮⡂⣙⢷⣕⠀⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠁⠨⢻⣷⡣⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠿⠘⣿⠀⠀⠀⠀⠀⠀⠀⠀⣻⣿⣿⣿⣿⣆⡄⠀⠀⢹⡇⡄⠀⠀⢸⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢘⣴⠟⠍⣊⣿⣿⣮⡠⣝⢿⣮⡠⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠑⠝⢿⣦⡠⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⣿⠀⠀⠀⠀⠀⠀⠀⢠⣿⠉⢦⣔⠄⣿⡀⠀⡀⣾⡇⠁⠀⠀⢨⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠸⣷⠾⠟⠋⠑⠒⢙⢷⣝⠰⣝⢿⣅⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠐⣝⢿⣮⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⢿⡆⠀⠀⠀⠀⠀⠀⡼⣿⣦⣼⣿⣷⣿⣥⣤⣵⢟⠁⠀⠀⠀⢸⡟⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠀⠈⠀⠀⠀⠀⠀⠑⢙⢿⣮⠑⡙⢷⣄⡢⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠀⡻⣿⣦⡢⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⢸⣧⠀⠀⠀⠀⠀⠀⠈⠊⠙⠻⣿⣻⣿⣟⡛⠉⠊⠀⠀⠀⡀⣼⡇⢿⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠑⡝⢷⣆⠐⣝⢿⣮⡢⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠈⡻⣿⣕⠆⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⢠⢿⣄⠀⠀⠀⠀⠀⠀⠀⠀⠀⣿⡏⣻⣿⣮⡢⠀⠀⠀⢠⢣⡿⠀⣿⢣⣤⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢄⣢⣬⣶⠿⡛⢿⣮⡲⣝⢿⣦⡢⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⢪⢿⣧⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠉⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⣷⠱⠹⣿⡿⣦⣔⣐⣴⣿⡁⠀⣿⢀⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠠⠄⢀⣐⣤⣢⠀⠀⠀⠤⢀⣠⣤⣴⣾⠿⣛⠍⠂⠁⠀⠱⠙⢿⣮⡳⡝⢿⣦⡲⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⣿⡆⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⣿⡆⠸⠙⣿⣎⢙⠛⠿⣿⣶⣤⣿⣸⡏⠄⠀⠀⠀⠀⢠⣴⣶⣶⣶⡶⠶⠾⠿⠿⡛⣽⣇⣤⣶⣾⡿⢿⣿⠻⣿⣄⢠⠀⠀⠀⠀⠀⠀⠀⠰⢝⢿⣮⡪⠛⢿⣮⡢⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠠⢄⣂⣬⣾⣿⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢿⣧⠀⠀⠈⢿⣆⢀⠀⢿⣏⣿⣿⣿⣿⣷⣶⣶⣶⣶⣾⣷⡀⡀⠀⠀⠀⠀⠀⠀⣳⡟⠛⠩⠉⠀⠈⠊⡻⣿⣬⠻⣷⡕⠄⠀⠀⠀⠀⠀⠀⠀⠁⡙⢿⣆⢱⡽⣷⣄⢀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠠⠄⣀⣬⣴⡿⠟⢛⣽⣿⠋⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠸⣿⡄⠀⠀⠘⣿⣎⢆⢏⣿⣿⣼⡟⠩⣢⡾⢯⠀⠀⠀⢝⢿⣅⠀⠀⢀⣒⣀⠀⣿⠁⠀⠀⠀⠀⠀⠀⠈⠮⠻⣷⣈⠻⣦⡱⡀⠀⠀⠀⠀⠀⠀⠀⠨⠻⣷⣍⡪⡻⣷⣤⡢⠀⠀⠀⠀⡀⢀⣢⣴⡶⢟⡛⢉⣢⣤⣾⡿⢟⠕⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠰⢻⣧⠀⠀⠀⠸⣿⣶⢟⢁⣿⡟⠛⠛⠫⠀⠀⠀⠀⠀⠀⠘⣿⣶⣿⠿⠟⠿⣿⣿⣆⠀⠀⠀⠀⠀⠀⠀⠀⠀⠪⡻⣾⡨⠻⣮⡐⡀⠀⠀⠀⠀⠀⠀⠘⠨⡻⢿⣮⡪⠛⠿⣷⣶⣶⣶⡾⢟⠫⢁⣠⣵⣾⠿⣿⠉⣿⠇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠰⢻⣧⠀⠀⠀⢹⣿⣱⠿⠫⠂⠀⠀⠀⠀⠀⠀⠀⠀⠰⣼⡿⡫⠒⠀⡀⠀⡀⢝⢿⣧⠀⠀⠀⠀⠀⠀⠀⠀⠀⠘⢜⢿⣄⡈⢿⣦⡀⢀⠀⠀⠀⠀⠀⠀⠀⠓⢙⠿⣷⣥⣐⣒⣂⣂⣤⣴⣾⠿⠛⠿⣷⣾⣿⢰⡿⡄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢫⠻⣧⡀⠀⠈⣿⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢰⣿⠳⠀⢐⣵⡾⠿⣮⣳⢣⢻⣇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠝⢷⣄⡝⢿⣦⡱⠀⠀⠀⠀⠀⠀⠀⠀⠀⠊⠙⠛⡻⣿⣛⢻⣿⠐⠁⠀⠀⠊⣿⡿⣼⣇⢀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠐⠩⢿⣦⣴⡿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⡇⠀⠀⢸⡏⠊⢘⢹⡇⠀⢸⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠝⢿⣤⠙⢿⣦⡣⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠙⠙⣷⡃⢿⡇⠀⠀⠀⠀⣿⡇⣿⠿⣷⣕⢄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠁⠂⠀⠚⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⡇⠀⠀⠸⣷⣄⣈⣿⡇⠀⢸⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠐⢝⢷⣤⡙⢿⣮⡂⠀⠀⠀⠀⠀⠀⠀⠀⠀⠘⡽⣧⡘⣿⡀⠀⠀⠀⣿⢿⡿⠀⠉⡻⣷⡄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠸⣿⣠⠀⠀⠝⠛⠛⠫⠂⠀⣿⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠑⢝⢿⣦⡹⢿⣮⡣⡀⠀⠀⠀⠀⠀⠀⠀⠰⡹⣧⠸⣧⢀⠀⠀⣿⣾⠃⠀⠀⠀⢘⣿⡄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠘⠹⣷⣝⠄⡀⠀⢀⡠⣈⣾⡿⠓⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠓⠝⢿⣦⡙⢿⣦⡠⡀⠀⠀⠀⠀⠀⠀⠁⠹⣧⣿⡎⠀⠘⠉⠛⠀⠀⠠⣠⣼⣿⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠪⡻⢿⣶⣶⣶⣾⡿⡫⠙⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠐⠝⢿⣦⣝⢿⣦⡂⡀⠀⠀⠀⠀⠀⠀⠘⠫⡟⠀⢀⠠⣀⣠⣴⡿⢟⣫⡿⡅⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠉⠁⠀⠈⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠑⢙⡻⣷⣝⢿⣮⣀⠄⠀⠀⠀⠀⠤⣀⣢⣬⡶⠿⠛⣉⣤⡾⣛⡍⠊⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠁⠨⡻⣷⣮⡛⠻⠶⠶⠶⠿⠛⠛⢉⣁⣬⡶⠟⠋⠑⠈⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠙⡻⢷⣶⣶⣶⣶⠶⠿⢛⡋⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
```

```
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠰⠦⣀⣠⣬⣽⣶⣾⣿⣿⠿⠿⠿⢿⣿⣿⣿⣿⣴⣶⣯⣤⡢⢤⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣤⢜⣯⣶⣿⣿⠿⠿⠛⠛⠭⠁⡌⣿⠈⠉⠉⠁⠀⠀⠀⠈⠉⠭⠛⠻⢿⣷⣫⣀⢤⡄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⡄⣫⣶⣿⢟⣧⠁⠐⠃⠀⠀⠀⠀⠀⡇⢿⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠓⢩⡻⢿⣿⣶⣝⡃⢀⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⢖⣴⣿⡿⣫⠒⠃⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣿⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠓⠊⢝⡻⣿⣷⣦⣔⠆⣀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢖⣵⣿⢟⠱⠎⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣿⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠰⠯⢛⠿⣿⣮⡂⣀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠠⣳⣿⢟⠅⠉⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠁⠮⠻⣿⣞⢤⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⡜⣼⣿⡃⠉⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⢝⢿⣷⡣⡄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢠⢘⣾⡿⣷⠃⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠘⢫⡻⣿⣜⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⡶⣰⣿⢟⠙⠂⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠙⣿⣧⡂⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⡶⣨⣾⡿⡳⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⡏⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠎⢿⣷⣔⠆⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢠⢜⣾⡿⡫⠈⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⡄⣼⡟⣿⣯⡠⡄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⢛⣵⣿⡟⡝⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢠⢱⣿⠈⢪⡻⣿⣮⣣⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⢐⣴⣿⢟⢹⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⣷⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⡈⣿⠇⠃⠀⠘⠊⢿⣷⠳⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⢈⣾⡿⡕⠀⢸⣷⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣀⣀⡀⣀⠀⠀⠀⠀⢸⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣀⣀⣀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⣹⡟⠀⠀⠀⠀⠀⢋⣿⣇⠆⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⣼⡿⠀⠁⠀⢸⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠠⠤⣀⣀⣤⣤⣽⣶⣶⣶⣾⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣷⣿⣿⢿⣷⣶⣶⣾⣤⣤⣔⣂⡢⠀⠀⠀⠀⠀⠀⠀⣄⣿⠃⠀⠀⠀⠀⠀⠸⢹⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢣⣿⣇⠀⠀⠀⠈⣿⠀⠀⠀⠀⠀⠀⣤⠤⣀⣭⣵⣶⣿⣿⠿⠿⠟⠛⠛⠭⠭⠉⠉⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠉⠉⠭⠝⠛⠛⠿⠿⣿⣿⣶⣮⣅⡠⢄⢠⣸⡟⡆⠀⠀⠀⠀⠀⠀⡎⣿⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⣿⠘⠀⠀⠀⠀⣿⡆⡄⢠⡤⣛⣥⣶⣿⠿⢟⣻⠉⠑⠒⠛⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠋⠀⠊⢩⣛⠿⢿⣷⣦⣿⢣⡅⠀⠀⠀⠀⠀⠀⠁⢻⣷⢀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣀⠀⠀⠀⠀⣿⡟⣀⠀⠀⠀⠘⢹⣇⢓⣴⣿⡿⣛⡍⠒⠂⠀⠀⣀⣀⣀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣀⠐⣒⣤⣤⣶⣶⣦⣤⣤⣔⣂⠀⣀⡒⢡⣛⢿⣷⣔⠆⡀⠀⠀⠀⢀⠀⣸⣯⣜⣒⣒⠀⣀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⡶⣢⣶⣾⣾⣿⣿⣿⣷⣶⣴⡆⠀⣰⣪⣿⡿⢟⠵⠀⠀⢀⠰⢖⣠⣤⣶⣶⣶⣶⣤⣔⡲⢀⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⡰⣢⣵⣿⣿⠿⠿⠛⠛⣻⠿⢿⣿⣿⣿⣶⣥⡲⣆⠳⢝⢿⣷⣅⢀⡀⠀⠘⣿⣿⣿⡿⣿⣿⣿⣶⣔⢆⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢰⢮⣾⣿⢟⠫⠭⠉⠩⡍⣿⣿⡃⠁⣜⣵⣿⠏⠄⠉⠀⡤⣀⣵⣾⣿⡿⠿⠛⠛⠙⠛⠿⣿⣿⣶⣅⢤⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢠⢞⣿⣿⠿⠫⠄⠈⠉⠀⠀⠉⠉⠀⠮⢛⢿⣿⣿⣿⣷⣔⠌⠁⢝⣿⣯⠃⠀⠰⢹⣿⡖⠀⠀⠀⠍⠻⣿⣯⢆⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢧⣿⡿⡅⠉⠀⠀⠀⠀⣼⣿⠇⢡⢨⣾⡟⣵⠁⠀⡤⣨⣾⣿⡿⢛⡅⠈⠁⠀⠀⠀⠈⠉⢰⡭⡻⣿⣷⣝⡄⠀⠀⠀⠀⠀⠀⠀⠀⠀⢠⣳⣿⡿⡳⠎⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠁⡽⣿⣷⡙⣿⣯⣣⠈⡌⢿⣷⣠⠀⠋⣿⣿⢠⠀⠀⠀⠁⠹⣿⣯⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠆⣿⣿⢱⠀⠀⠀⠀⢰⣰⣿⡏⠆⢯⣿⡟⡞⠀⡠⣠⣾⣿⣿⢿⡜⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠛⢪⢻⣿⣦⠀⠀⠀⠀⠀⠀⠀⠀⠸⣰⣿⡟⠘⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠘⢘⢿⣿⡌⣻⣷⡄⡄⢋⢿⣷⢣⡀⢸⣿⣇⣭⣛⢀⡀⢰⢻⣿⡄⡄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⣿⡇⠀⠀⡶⣤⣶⣶⣿⡿⣆⢆⣿⡟⠚⠀⡶⣵⣿⣿⣿⣣⠃⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠐⡽⣿⣧⠆⠀⠀⠀⠀⠀⠀⢰⣿⡟⡆⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢊⣿⣷⣁⢻⣿⡵⠘⠋⣿⣧⢃⠀⢿⣿⣿⣿⣷⡵⠀⠘⣿⣇⠃⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣼⣿⠀⠀⠀⢨⣿⣿⣿⣿⢳⡙⣾⡿⡄⠀⢀⣾⡿⣽⣿⠳⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠰⠹⣿⣇⢀⠀⠀⠀⠀⣄⣿⡿⠘⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠸⠸⣿⣏⠃⢿⣷⢠⠀⡜⣿⡞⠀⠸⣿⣿⣿⣿⡇⠀⠀⣿⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣿⣿⠀⠀⠀⢸⣿⣿⣿⡏⠈⢹⣿⠃⠁⡄⣼⡿⢹⣿⠇⠇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠰⢻⣿⡼⠀⠀⠀⠀⢸⣿⣇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⡤⣠⣤⣤⣀⢄⠀⢿⣿⡀⠞⣿⡇⠀⠁⢻⣿⠸⠀⢿⣿⣿⣿⢇⠀⠀⣿⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣿⣿⠀⠀⠀⠞⢿⣿⣿⠃⡄⣿⡏⠀⠀⣹⣿⠃⣿⣿⠰⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣤⣘⣭⣭⣭⡀⡄⡞⣿⣇⠀⠀⠀⠀⣿⣿⠈⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢠⢠⣾⣿⣿⣿⣿⣷⡅⢸⣿⡇⢠⢛⣷⠀⠀⠘⣿⡇⡄⢸⣿⡿⣫⠏⠀⢀⣿⡿⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠘⢸⣿⡞⠀⠀⠀⠋⣿⣿⡀⢸⣿⢣⠀⢀⣿⡏⢰⣿⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠸⣽⣿⣿⣿⣿⣿⣦⠀⣿⣿⠀⠀⠀⠀⣿⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣿⣿⣿⣿⣿⣿⣿⣷⠈⣿⡇⠀⢸⣿⠀⠀⠀⢿⣷⠃⡜⢿⡆⠀⠀⡰⣼⣿⠇⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⢿⣿⡴⡀⠀⢰⣿⡆⠃⣼⣿⠀⢀⢸⣿⠁⢸⣿⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠰⣸⣿⣿⣿⣿⣿⣿⣿⡇⢸⣿⠀⠀⠀⠀⣿⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⣿⣿⣿⣿⣿⢿⣿⣿⡆⣿⡇⠀⠘⣿⡇⠀⠀⢸⣿⠀⠀⣿⡇⠰⣢⣮⣿⢏⠃⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢎⢿⣿⣦⡲⢸⣿⠇⠀⣿⡇⡇⠈⣼⣿⡀⢸⣿⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣿⣿⣿⣿⣿⡿⣿⣿⣿⢸⣿⠀⠀⠀⠀⣿⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣸⣿⣿⣿⣿⣇⢪⣿⣿⢃⣿⡇⠀⠀⣿⡇⠀⠀⠸⣿⣆⣀⣿⣷⣿⣿⣿⠳⠈⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠱⢹⣿⣿⣿⣿⣬⣥⣿⡇⠀⠀⣿⡇⠁⢸⣿⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣿⣿⣿⣿⣿⣌⣼⣿⡟⣸⣿⠀⠀⠀⠀⢿⣿⢠⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢡⢿⣿⣿⣿⣿⣿⣿⣟⢸⣿⡇⠀⠀⣿⡇⠀⠀⡆⣿⡿⠿⠿⠿⠟⢻⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⣿⢛⠛⣛⡛⢻⣿⠁⠀⠀⣿⡇⠀⡜⣿⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠸⣿⣿⣿⣿⣿⣿⣿⡃⣿⣿⠀⠀⠀⠀⢸⣿⡏⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠘⢫⡻⣿⣿⣿⣿⢟⡞⢾⣿⠀⠀⢀⣿⡇⠀⠀⠆⣿⡇⠉⠃⠀⠀⢸⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⣿⠀⠀⠀⠀⢸⣿⠀⠀⠀⣿⣇⠆⠃⣿⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠘⣝⢿⣿⣿⣿⡿⡃⢱⣿⡏⠀⠀⠀⠀⠀⣿⣿⡰⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠘⠂⠉⠉⠒⢰⢳⣿⡏⠀⢀⢸⡿⠀⠀⠀⠀⣿⡇⠀⠀⠀⠀⢸⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⣿⡴⠀⠀⠀⢸⣟⠀⠀⠰⢹⣿⠀⠀⠸⣿⣇⡆⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠐⠊⠉⠳⢀⡀⣾⣿⠱⠀⠀⠀⠀⠀⠘⣿⣧⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⢦⣿⡿⡄⠀⡘⣾⡿⡄⠀⠀⡆⣿⡇⠀⠀⠀⢰⣸⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⢿⣧⠀⠀⠀⢸⣿⡄⠀⠀⡸⣿⡆⡀⠀⢻⣿⣆⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠸⣽⣿⠇⡦⢄⣀⣀⣀⣀⡼⠹⣿⣧⣠⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢠⢪⣿⡿⠱⠁⠀⣱⣾⣳⠁⠀⠀⢠⣽⡇⠀⠀⠀⢆⣿⡋⠇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠘⢿⣷⣝⣀⠄⣿⡇⠀⠀⠱⢻⣷⢡⠀⢦⢿⣿⣞⠄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣼⣿⠯⣣⣾⣿⣿⣿⣿⣿⣿⣶⣝⣿⣷⣅⢤⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢠⢄⣵⣿⡿⠁⠀⢠⣳⣿⠏⠉⠀⠀⢠⢸⣿⣶⣶⣶⣾⣿⣿⢸⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣼⣿⠻⠿⣿⣿⣧⠀⠀⠀⠈⣿⣧⢧⡀⢣⠻⣿⣧⡻⡄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⡤⣫⣾⣿⢯⣸⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⡎⡻⣿⣷⣝⡃⠠⡄⠀⠀⠀⣀⠤⣛⣵⣿⡿⣫⠀⢀⢜⣴⣿⠋⠀⠀⠀⠀⡜⢿⡏⡍⠉⠉⠉⢸⣿⠘⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣿⡇⠃⠀⠀⡼⣿⡆⡀⠀⠀⢚⢿⣷⡳⡀⠘⣝⢿⣿⣦⣔⡶⢀⣀⣀⣀⣀⠀⢖⣦⣾⣿⡿⡕⣣⣽⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣦⣪⡻⣿⣿⣿⣶⣶⣶⣶⣶⣿⣿⠿⣫⣚⠃⣒⣴⣿⢟⠕⠀⠀⠀⠀⡀⣽⣿⡅⠀⠀⠀⠀⣼⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢠⣿⡇⠀⠀⠀⠀⣻⣿⡁⡀⠀⠀⠯⡻⣿⣦⡲⢀⡰⠝⡻⣿⣿⣷⣶⣶⣶⣶⣿⣿⣿⡿⣫⣪⣾⣿⢟⡻⢿⣿⣿⣿⣿⣿⣿⡿⣫⢙⢿⣿⣮⡲⠝⡻⢿⣿⣿⣿⣿⣭⣥⣤⣴⣶⢿⡿⡛⠵⠇⠀⠀⠀⠀⡰⣹⣿⠃⠀⠀⠀⠀⠀⣿⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⣿⠀⠀⠀⠀⠀⠱⢻⣷⡡⠀⠀⠀⠉⠬⡻⣿⣴⣭⣅⣉⡠⠭⢝⣛⣛⣿⣿⣿⠿⠫⠀⣱⣿⡟⠵⠉⠉⠁⠮⠭⠙⠫⠭⠅⠈⠉⠈⠁⢝⣿⣶⠃⠉⠀⠪⠭⠝⠛⠛⠛⠛⠫⠭⠄⠈⠁⠀⠀⠀⠀⠀⡜⣽⣿⠳⠇⠀⠀⠀⠀⠀⣿⣧⢤⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠘⣿⡇⠀⠀⠀⠀⠀⣧⣻⣷⡝⡄⠀⠀⠀⠉⠀⣭⡛⠿⠿⣿⣿⣿⠿⠿⠛⢫⠅⠉⠠⣳⣿⡟⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⢸⣿⣇⢠⡄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢠⢘⣾⣿⣿⠀⠀⠀⠀⠀⠀⠀⣞⣿⣯⠇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣿⡇⡀⠀⠀⠀⠀⠀⢳⡽⣿⣮⢀⡀⠀⠀⠀⠀⠀⠀⠘⠓⠒⠂⠀⠀⠀⠀⢀⢟⣼⣿⣿⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⣿⣿⣷⣮⡓⢀⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣀⢟⣴⣿⢟⢸⣿⡀⠀⠀⠀⠀⠀⠀⠘⠘⣿⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣿⡇⡇⠀⠀⠀⠀⠀⠀⠘⢘⢿⣷⣕⠆⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣀⠀⣢⣴⣿⢟⢹⣿⡆⣀⠀⠀⣀⡀⠀⢀⣀⣀⡀⠀⢀⣀⡀⣀⡐⣼⣿⠑⢩⡻⢿⣷⣦⣄⣒⡀⠀⠀⠀⠀⠰⣒⣬⣶⣿⢟⡕⠀⠈⣿⡇⠀⠀⠀⠀⠀⠀⠀⠃⣿⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢻⣿⠀⠀⠀⠀⠀⠀⠀⠀⠈⣸⣿⢿⣿⣮⣔⡲⠆⠀⠀⠶⣖⢂⣤⣶⣿⡿⡋⠵⠁⠏⢿⣿⣯⣤⣤⣵⣾⣿⣿⣿⢿⣿⣿⣷⣶⣦⣶⣾⣿⠏⠆⠀⠈⠀⠭⠛⡻⠿⣿⣿⣿⣿⣿⣿⡿⢟⠫⠶⠁⠀⠀⠀⣿⡇⠃⠀⠀⠀⠀⠀⠀⠀⢿⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⣿⡏⠁⠮⠛⠿⢿⣿⣿⣿⣿⡿⠿⠛⠫⠅⠈⠁⠀⠀⠀⠨⠛⠿⣿⡿⠟⠛⠍⢰⣿⡇⠈⠭⠝⢻⣿⡟⠛⠵⠁⠀⠀⠀⠀⠀⠀⠉⠉⠀⠀⠀⠀⠀⠀⠈⠉⠀⠀⠀⠀⠀⠀⢹⣿⣠⠀⠀⠀⠀⠀⠀⠀⢸⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠸⣿⡄⠀⠀⠀⠀⠀⠀⠀⢰⡿⢇⠀⠀⠀⠈⠁⠀⠂⠀⠀⠈⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣿⡇⠀⠀⠀⢸⣿⡇⠀⠀⠀⢸⣿⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠏⣿⣇⠀⠀⠀⠀⠀⠀⠀⣼⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠃⣿⡇⠀⠀⠀⠀⠀⠀⠀⢸⣿⠘⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⣿⡇⠀⠀⠀⢸⣿⡇⠀⠀⠀⠀⣿⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢹⣿⠀⠀⠀⠀⠀⠀⠀⣿⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣿⡆⠀⠀⠀⠀⠀⠀⠀⢸⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⣿⡇⠀⠀⠀⢸⣿⡇⠀⠀⠀⠀⣿⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⣿⠀⠀⠀⠀⠀⠀⢃⣿⣇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣿⡇⠀⠀⠀⠀⠀⠀⠀⢸⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⣿⡇⠀⠀⠀⢸⣿⡃⠀⠀⠀⢀⣿⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⣿⠀⠀⠀⠀⠀⢰⣸⣿⠈⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢇⣿⡇⠀⠀⠀⠀⠀⠀⠀⢸⣿⢠⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⣿⡇⡄⠀⡜⣽⣿⣧⡠⠄⡤⣸⣿⣇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⣿⢠⠀⠀⠀⠀⣤⣿⣆⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⢠⠤⢤⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢠⢘⣿⠁⠀⠀⠀⠀⠀⠀⠀⡜⣿⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢣⢾⣿⣶⣶⣽⣿⢟⢿⣿⣷⣾⣿⠟⠈⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣼⡿⠈⠀⠀⠀⡄⣼⡿⣬⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⢎⣿⣷⡄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⣿⡟⡆⠀⠀⠀⠀⠀⠀⠀⢰⣿⢧⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠐⣝⣛⣛⡋⠑⠀⠑⠉⠙⠛⠑⠂⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢆⣿⡇⠀⠀⠀⢀⢱⣿⢧⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⡀⠀⠀⠀⣀
⣆⣼⣿⢻⣿⡰⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢠⢰⣿⠃⠀⠀⠀⠀⠀⠀⢀⢀⣿⡟⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⣿⠱⠀⠀⠀⠈⣾⡟⡄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⠰⣪⣾⣿⣿⣿⣮
⣿⡝⠵⡎⣿⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⣾⡟⠆⠀⠀⠀⠀⠀⠀⢌⣾⡿⡅⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⣿⠀⠀⠀⠀⢀⣿⣇⠃⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢨⣾⣿⢛⣭⣴⢹⣿
⣿⣇⠀⠁⣿⣇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢰⣿⢳⠀⠀⠀⠀⠀⠠⣫⡿⣟⡍⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢿⣿⠀⠀⠀⠀⠈⡼⣿⣮⡠⡄⠀⠀⠀⠀⠀⠀⠀⠀⠠⣰⣿⢿⣿⣿⢟⣥⣿⡿
⠸⣿⡾⠀⢹⣿⠘⠀⠀⠀⠀⠀⠀⠀⠀⠀⣀⡀⠠⣠⣿⡏⠀⠀⠀⠀⢀⣀⣴⣿⣿⠚⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⡼⣿⣞⠀⠀⠀⠀⠀⢨⡻⣾⣮⡠⡀⠀⠀⠀⠀⠀⡀⣴⣿⢫⡸⣿⣷⣿⡿⣫⠘
⠘⢹⣿⡴⡸⣿⡜⠀⠀⢐⣢⣤⣶⣶⣶⣶⣶⣾⣿⡿⣟⢂⣀⠀⠀⠐⣪⣾⡿⣿⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢙⣿⣧⡰⢀⡀⠀⠀⠛⢈⡻⣿⣦⣲⡀⠀⠀⠀⣹⣿⠃⣪⣾⡿⣛⠍⠂⠀⠀
⠀⢠⣻⣿⡱⡻⣿⣷⣿⣿⠿⡛⠨⡭⠩⠭⢭⠽⠂⡀⢔⣬⣶⣾⣿⣿⠿⠫⠂⣿⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠾⡻⣿⣷⣕⢦⠀⠀⠀⠀⠊⢿⣷⡵⢆⠰⢦⣿⠏⣰⣿⠏⠾⠁⠀⠀⠀⠀
⠀⠈⠱⣻⣿⣝⠤⠍⢡⠤⣩⣵⣶⣴⣶⣶⣶⣶⣶⣶⣿⠟⠫⠅⠀⠀⠈⠀⠀⣿⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠁⣿⣿⢿⣷⡁⢤⠀⠀⠀⠱⡫⣿⣶⣶⣿⢟⢲⣿⠇⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠁⣝⢿⣿⣶⣶⣿⠿⠻⡍⠉⠉⠉⠉⠉⠉⠉⠑⠁⠀⠀⠀⠀⠀⠀⠀⣿⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣿⣿⠐⣝⢿⣶⣜⡣⠀⠀⠉⠈⠉⠉⠁⣭⣼⣿⠰⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠘⠒⠉⠉⠒⠛⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣿⣟⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣿⣿⠀⠀⠓⣝⠿⣿⣦⣬⣚⣂⠀⢀⡸⣱⣟⢧⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣿⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣿⣿⠀⠀⠀⠀⠀⠊⠛⣻⠿⠿⣿⣷⣾⡿⡳⠃⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⣽⣿⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣿⣿⠀⠀⠀⠀⠀⠀⠀⠉⠀⠁⠰⠭⠩⠾⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠁⠉⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣿⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
```

## Acknowledgement

Project inspired by https://github.com/asciimoo/drawille and [Exrook's go port](https://github.com/exrook/drawille-go).
