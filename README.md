# PokeBlazor

A simple example of how Blazor can be used to build single page applications against a known API - in this case the Pokemon API

## Licence Used
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

See the contents of the LICENSE file for details.

## Support This Project

If you have found this project helpful, either as a library that you use or as a learning tool, please consider buying me a coffee:

<a href="https://www.buymeacoffee.com/dotnetcoreshow" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important" ></a>

## Pull Requests

[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)

Pull requests are welcome, but please take a moment to read the Code of Conduct before submitting them or commenting on any work in this repo.

## Docker Image

PokeBlazor is now available on docker hub at [gaprogman/pokeblazor](https://hub.docker.com/r/gaprogman/pokeblazor/). To pull the latest version of the image, run the following command:

```
docker pull gaprogman/pokeblazor
```

(the above assumes that you have docker installed and set up on your machine)

To run the image, issue the following command:

```
docker run -d -p 8080:5000 --name pokeblazor gaprogman/pokeblazor
```

The above command will:

- Start a new container called `pokeblazor`
- Run the `gaprogman/pokeblazor` image within it
- Detach the terminal from the new container
- Use port 8080 on the host and port 5000 on the container

## Requirements

The following software needs to be installed:

- [.NET Core SDK 2.1 or greater](https://dot.net/core)
- [Visual Studio 15.7 or greater](https://www.visualstudio.com/vs/preview)

## Building and Running the Project

If the sln file is opened with Visual Studio 15.7 or greater, then hitting Ctrl+F5 (or just F5) will start PokeBlazor.Server, which will start the application.

If running from the command line, you will need to cd into the PokeBlazor.Server directory and run:

``` shell
dotnet run
```

## Publishing

A Dockerfile has been provided, so you can publish and run a container like so. The example below is accessible on http://localhost:8080

``` shell
docker build -t pokeblazor .
docker run -p 8080:80 pokeblazor
```
