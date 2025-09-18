<!-- SPDX-License-Identifier: Apache-2.0 -->
<!-- Copyright Contributors to the ACES Project -->

# ACES Look Transforms

[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) [![CLA
assistant](https://cla-assistant.io/readme/badge/ampas/aces-look)](https://cla-assistant.io/ampas/aces-look)

ACES Look Transforms, or Look Modification Transforms (LMTs), provide a
mechasnism for applying creative or stylistic adjustments to ACES images. A Look
Transform modifies the default appearance produced by an Output Transform,
enabling customized looks that can be reused as alterative starting points on
ACES projects.

Formally, LMTs are defined as ACES-to-ACES transformations, though intermediate
encodings may be used internally when specific color operations require it. In
the process diagram, the output of an LMT is referred to as ACES' ("ACES
prime"), which is subsequently processed Output Transform.  

                |---------|            |---------|
                |         |            |         |
      ACES ---->|  Look   |--- ACES'-->| Output  |--->   display 
                |Transform|            |Transform|     code values
                |         |            |         |
                |---------|            |---------|


More information about designing and using Look Transforms can be found in the
[ACES Documentation](docs.acescentral.com).

## Contributing

ACES depends on community participation. Developers, manufacturers, and end
users are encouraged to contribute code, bug fixes, documentation, and other
technical artifacts.

All contributors must have a signed Contributor License Agreement (CLA) on file
to ensure that the project can freely use your contributions. 

See [CONTRIBUTING.md](./CONTRIBUTING.md) for more details.

## Governance

This repository is a submodule of the ACES project, hosted by the ASWF. Details
about how the project operates can be found in the
[GOVERNANCE.md](https://github.com/ampas/aces/blob/main/GOVERNANCE.md) file in
the top-level ACES repository.

## Reporting Issues

To report a problem with Look Transfoms, please open an
[issue](https://github.com/ampas/aces-look/issues).

If the issue is senstive in nature or a security related issue, please do not
report in the issue tracker. Instead refer to [SECURITY.md](SECURITY.md) for
more information about the project security policy.

## License

The ACES Project is licensed under the [Apache 2.0 license](./LICENSE).