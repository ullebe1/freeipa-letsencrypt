# FreeIPA Let's Encrypt
This container expands the official FreeIPA container(s) with the needed services to automatically enable LetsEncrypt certificates for both LDAPS and HTTPS. It does not contain any functionality to obtain said certificates, rather they should be obtained using your preferred method and mounted into the container. 

This container is currently only available for FreeIPA based on CentOS 8, but more flavors can be enable upon request.

# How to use
To use, simply mount the LetsEncrypt folder containing your certificates to `/etc/letsencrypt/` in the container. Changes to the certificates will automatically be detected and applied immediately.

This container requires the domain of your certificate to match the hostname of your container, which is also the way recommended by the upstream FreeIPA container.

# Notes

## Status

This container is currently EXPERIMENTAL, so please don't use it where you need to be able to rely on it and/or where it matters if it destroys everything it touches. 


## The license for the contents of this Git repository

MIT License

Copyright (c) 2021 Ulrik Boll Djurtoft

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
