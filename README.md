# revanced-creator
this script first downloads the latest [revanced-cli](https://github.com/revanced/revanced-cli), [revanced-patches](https://github.com/revanced/revanced-patches) and [revanced-integrations](https://github.com/revanced/revanced-integrations). then it downloads the latest supported youtube version and patches it according to [revanced-documentation](https://github.com/revanced/revanced-documentation)
## deps
- curl(curl is required to get latest versions of revanced-*)
- (optional)awk
- java(17)
- grep
## usage
```
$ mkdir -p revanced
$ cd revanced
$ sh -c "$(curl https://raw.githubusercontent.com/XDream8/revanced-creator/main/patch.sh)"
```
* or
```sh
$ git clone https://github.com/XDream8/revanced-creator
$ cd revanced-creator
$ chmod +x patch.sh
$ ./patch.sh
```
### options
#### nonroot(defaults to 1)
```sh
$ nonroot=1 ./patch.sh
```
#### downloader
```sh
$ downloader="axel -n 16" ./patch.sh
```
#### or you can use these two options together
```sh
$ nonroot=1 downloader="axel -n 16" ./patch.sh
```
