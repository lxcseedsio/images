# lxcseeds.io public images

Official public http://lxcseeds.io lxc images for lxd servers

## Installation

Install using plain lxd command.

First add lxcseeds.io remote lxd server :

``lxc remote add lxcseeds lxcseeds.io:8443 --public``

Then check for existing images :

``lxc image list lxcseeds:``

You can install images using :

``lxc launch lxcseeds:[image] [containerName]``

You can get extra infos on images using :

``lxc image info lxcseeds:[image]``

## Example

``lxc launch lxcseeds:wily/camp/amd64 mycontainer``

## Search for images

Images can be searched on those fields :
- description : description of the image
- type : type can be micro, fat, infra, devstack or other
- tags : installed components (apache, php, ...)

Examples :

``lxc image list lxcseeds: type=fat``

``lxc image list lxcseeds: apache=True``

## Propose and votes

You can propose and vote for containers you'd like to find using Twitter to @lxcseedsio with hashtag #seedwanted

## Contributing

Feel free to propose PR with your own .yml file.
1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request

## Credits

Credits lxcsseds.io

## License

MIT
