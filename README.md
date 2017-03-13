# Docker for LIMS Doxygen

This is the PHP container for documenting the Stowers in-house LIMS application. Based on the [official PHP](https://hub.docker.com/_/php/) container.

## Requires

* Docker v1.12+

## Includes
### Included Applications

* **php** - Needed for doxygen to scan the source
* **graphvis** - Needed for pretty pictures in Doxygen
* **doxygen** - The documentor

## To Run

Run the following in the root of your PHP code base.

```bash
docker run -v /path/to/src:/src --rm stowers/php-doxygen doxygen/Doxyfile
```

## Contributions

If you see something in this Dockerfile that can be done better, please submit a pull request.
