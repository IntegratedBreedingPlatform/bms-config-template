bms-config-template
=========

Aggregates all BMS modules and provides template configuration for building.

## Installation

Clone the repo and submodules in the same directory. Follow installation instructions in [BMS Manual setup]

## Usage

Setup database connection properties (db.host, etc.) in template/application.properties.

Build BMS modules:
```bash
mvn clean install -DskipTests -Duser.name=template
```
Or you can copy the template directory to a folder named as your system user name and simply run
```bash
mvn clean install -DskipTests 
```

On successful build, `.war` files will be created in `target` folder under each web application project directory. 
Deploy `.war` files to tomcat/webapp folder.

## TODO
- [ ] Enable tests

[BMS Manual setup]: https://github.com/IntegratedBreedingPlatform/Documentation/wiki/Manual-setup
