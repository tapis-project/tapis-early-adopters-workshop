## Container Support

Container technology significantly improves the portability and reproducibility of general
applications. However, adoption within the scientific computing community has lagged behind
industry. The primary reason is that containers cannot easily encapsulate all the dependencies
of scientific code running in customized, heterogeneous environments. Scientific computations
often rely on specialized hardware and custom software that cannot be captured within a
container. This includes requirements such as MPI, networking, mathematical and GPU libraries,
and specialized workflow managers. Additionally, the container runtime itself becomes a
dependency for an application that relies on a specific version, configuration or capability
of the runtime. <br/>

Our strategy with Tapis therefore is to augment container technology with metadata captured
by the platform. This metadata will describe requirements of applications as well as capabilities
of different execution environments. These abstractions are based on our experience running
containerized workloads in a variety of contexts. The execution system capabilities and
application requirements will allow the applications and jobs components of Tapis to support
containers as first class objects leading to improved flexibility when scheduling computational
workloads as well as greater portability and reproducibility when executing them. <br/>

[Container Support Slides](https://docs.google.com/presentation/d/160oYNFl5YAjWbs9thy6T9RLgX5o0xosQkfAjTCLA3r4/edit?usp=sharing)
