# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.1.9] - 2021-04-20

### Changed
- updated dependency versions

## [0.1.8] - 2021

### Changed
- renamed `logging.py` to `logger.py` to avoid colliding with the standard module name
- alter how the PED file is written to: for whatever reason, `Path().write_text()` was not working
  but using a open file context manager with `writelines()` does.
- make sure we bail out prematurely if there is a mismatch between the PED file and MAP file

## [0.1.7] - 2021-02-22

### Added
- CHANGELOG.md
- more logging info

### Fixed
- add missing import of liftPed to plinkliftover.__main__ from plinkliftover.liftover
- if the liftOver executable cannot be found, raise an error

## [0.1.6] - 2021-02-22

### Fixed
- replace `set` and `tuple` in type hints with their `typing.Set` and `typing.Tuple` counterparts


[0.1.9]: https://github.com/olivierlacan/keep-a-changelog/compare/0.1.8...0.1.9
[0.1.8]: https://github.com/olivierlacan/keep-a-changelog/compare/0.1.7...0.1.8
[0.1.7]: https://github.com/olivierlacan/keep-a-changelog/compare/0.1.6...0.1.7
[0.1.6]: https://github.com/olivierlacan/keep-a-changelog/compare/0.1.6...0.1.6
[0.1.5]: https://github.com/olivierlacan/keep-a-changelog/releases/tag/0.1.5
