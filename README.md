# OTP-PlantUML

![OTP diagram](http://www.plantuml.com/plantuml/png/hPBFRe9048VlFCN6dYrMRJKD4WN30rHlRKEsC182x93PfNzgVFSkbD15JBnq3cpopUoNtsnOIyL9LKLkDIMpL9ISUC5YEF0gLtluL9iyJKG1Gh58Vu3CiKf2n2KuZgnAeFTK8hakErfCrqxF0ggl4W8KoiSSYTq4JJNzozJZKPOGLY9kU_FPShkz_-qXnK0jd_cBm9zOfujnFf0o-FSea-Lykl26KIQBcVSGw2XcjLdOQBNozFaYRDkHwJSytatT8me83qYXFa-ENMFNjaVix1svP6_wwhdgTgT7W7h6vmH4A1l-QWYxb-XaxT30-GGbakexDrgghkYekJUCsEtHNtpFPMOqhoyV_a7BgW4RZyr53DQbwTX0i0OHrt_x3m00 "OTP Diagrams")

OTP-PlantUML is a attempt to use [PlantUML](http://en.plantuml.com/) and create some diagrams that fit the ideas found here [Erlang/OTP](http://erlang.org/doc/index.html). The intention is to get easy building documentation around Erlang and Elixir using OTP principles.

## Diagrams

* OTP Supervisor tree, a supervisor tree witch supervisors and workers can be draw using OTP-PlantUML. Additional stereotype were provided if you need to describe a bit more in detail each process. Right now the following stereotype exists: gen_server, gen_event, gen_statem, Agent, Task, Registry, Supervisor, TaskSupervisor

## How to use

The file `OTP.iuml` is the main file which needs to be include using one of the following methods:

* To be independent of any internet connectifity, download the file `OTP.iuml` found in the `root` and reference it locally with

```c#
!include path/to/OTP.iuml
```

* If you want to use the always up-to-date version in this repo, use the following:
```c#
!include https://raw.githubusercontent.com/joaohf/OTP-PlantUML/master/OTP.iuml
```

See [samples](samples) about how to use these diagrams.

## Contribute

This repository accepts features and improvements.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.