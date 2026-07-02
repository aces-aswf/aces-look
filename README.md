<!-- SPDX-License-Identifier: Apache-2.0 -->
<!-- Copyright Contributors to the ACES Project -->

# ACES Look Transforms

[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
[![CLA
assistant](https://cla-assistant.io/readme/badge/aces-aswf/aces-look)](https://cla-assistant.io/aces-aswf/aces-look)

ACES Look Transforms, or Look Modification Transforms (LMTs), provide a
mechanism for applying creative or stylistic adjustments to ACES images. A Look
Transform modifies the default appearance produced by an Output Transform,
enabling customized looks that can be reused as alterative starting points on
ACES projects.

Formally, LMTs are defined as ACES-to-ACES transformations, though intermediate
encodings may be used internally when specific color operations require it. In
the process diagram, the output of an LMT is referred to as ACES' ("ACES
prime"), which is subsequently processed Output Transform.  

``` mermaid
flowchart LR
    A["ACES"]
    B["Look
    Transform"]
    C["ACES'"]
    D["Output
    Transform"]
    E["Display
    Code Values"]

    A --> B --> C --> D --> E

    %% Define class with no border
    classDef noBorder stroke:none,stroke-width:0px,fill:none;
    
    %% Apply class
    class A,C,E noBorder;
```

More information about designing and using Look Transforms can be found in the
[ACES Documentation](https://docs.acescentral.com/).

## Contributing

ACES depends on community participation. Developers, manufacturers, and end
users are encouraged to contribute code, bug fixes, documentation, and other
technical artifacts.

All contributors must have a signed Contributor License Agreement (CLA) on file
to ensure that the project can freely use your contributions. 

See [CONTRIBUTING](https://github.com/aces-aswf/.github/blob/main/CONTRIBUTING.md) for more details.

## Governance

This repository is a submodule of the ACES project, which is itslef governed by the
Academy Software Foundation.

For details about how the ACES project operates, please see
[GOVERNANCE](https://github.com/aces-aswf/.github/blob/main/GOVERNANCE.md).

## Reporting Issues

To report a problem with Look Transforms, please open an
[issue](https://github.com/aces-aswf/aces-look/issues).

If the issue is senstive in nature or a security related issue, please do not
report in the issue tracker. Instead refer to [SECURITY](https://github.com/aces-aswf/.github/blob/main/SECURITY.md)
for more information about the project security policy.

## License

The ACES Project is licensed under the [Apache 2.0 license](./LICENSE).
