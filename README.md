# Excalibur

Personal dashboards using GrimoireLab

* [Github Issues](github-issues.png)
* [Github Pull Requests](github-pr.png) 


## Usage

### Local

* Install dependancies :

        $ python3 -m venv venv
        $ source venv/bin/activate
        $ pip3 install --upgrade pip
        $ pip3 install --upgrade setuptools
        $ pip3 install --upgrade wheel
        $ pip3 install grimoirelab

* Start services :

        $ docker run -p 127.0.0.1:9200:9200 -p 127.0.0.1:5601:5601 \
            -v $(pwd)/credentials.cfg:/override.cfg \
            -v $(pwd)/projects.json:/projects.json \
            grimoirelab/full

Kibiter is available : `http://localhost:5601`


## Contributing

Voir [CONTRIBUTING](CONTRIBUTING.md).

## License

[LICENSE](LICENSE) pour la license.

## Changelog

See [Changelog](ChangeLog.md) 

## Contact

Nicolas Lamirault <nicolas.lamirault@gmail.com>
