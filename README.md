# OTP-PlantUML

OTP-PlantUML is a attempt to use [PlantUML](http://en.plantuml.com/) and create some diagrams that fit the ideas found here [OTP Design Principles User's Guide](https://erlang.org/doc/design_principles/users_guide.html). The intention is to get easy building documentation around Erlang and Elixir using OTP principles.

## Diagrams

* OTP Supervisor tree, a supervisor tree which supervisors and workers can drawing using PlantUML. Additional stereotype were provided if you need to describe a bit more in detail each process. Right now the following stereotype exists: gen_server, gen_event, gen_statem, Agent, Task, Registry, Supervisor, TaskSupervisor:

![OTP Supervisor](http://www.plantuml.com/plantuml/png/hPBFRe9048VlFCN6dYrMRJKD4WN30rHlRKEsC182x93PfNzgVFSkbD15JBnq3cpopUoNtsnOIyL9LKLkDIMpL9ISUC5YEF0gLtluL9iyJKG1Gh58Vu3CiKf2n2KuZgnAeFTK8hakErfCrqxF0ggl4W8KoiSSYTq4JJNzozJZKPOGLY9kU_FPShkz_-qXnK0jd_cBm9zOfujnFf0o-FSea-Lykl26KIQBcVSGw2XcjLdOQBNozFaYRDkHwJSytatT8me83qYXFa-ENMFNjaVix1svP6_wwhdgTgT7W7h6vmH4A1l-QWYxb-XaxT30-GGbakexDrgghkYekJUCsEtHNtpFPMOqhoyV_a7BgW4RZyr53DQbwTX0i0OHrt_x3m00 "OTP Diagrams")

* OTP Sequence, sequence diagram with additional participants using stereotype and allowing sending messages, calling _cast_ and _call_:

![OTP Sequence](http://www.plantuml.com/plantuml/png/hLBBQiCm4BphAvRqd1BYj0x1cDGE_e7aNXHhumhRMY6jIqhflrTnKr0V8HGwXuNPdHa6eRLdwNZeEp72jzfOwMGF2Wzow7Y7HtxeT6DwD0nr6EXYMPYiQssbuIppWqNth3svF8TN0G7Re4VY5uiL6Iwf8mStrOZn_lksa7NRE1gCEjyMoNApkVkuaLFeplkaJAjo9jukLFhV4hFbOfuMFqlCqgIuhqubdhH2E13ndeuYGbnfKaYFjzlmKEWc83ti0t_q8uSiWmRD9ylphyuTsTZ8P2_wH9mwpMFj2hJHBABDD0XY_GgelPum_sl4jmn6prSaFZ0XrcZKwOU-0m00 "OTP Sequence")

## How to use

There are two plantuml include files (iuml):

* `OTP_SupervisorTree.iuml`
* `OTP_Sequence.iuml`

Each include file has macros which defines the _diagram_type_.

You need to include one of these two files using one of the following methods:

* To be independent of any internet connectivity, download the file respective `.iuml` found in the `root` and reference it locally with

```c#
!include path/to/OTP_<diagram_type>.iuml
```

* If you want to use the always up-to-date version in this repo, use the following:
```c#
!include https://raw.githubusercontent.com/joaohf/OTP-PlantUML/master/OTP_<diagram_type>.iuml
```

See [samples](samples) about how to use these diagrams.

## Contribute

This repository accepts features and improvements.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## References

* [C4-PlantUML](https://github.com/RicardoNiepel/C4-PlantUML)