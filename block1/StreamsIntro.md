## Streams API

The Tapis v3 **Streams API** provides a **production-quality** service that builds on top of the [CHORDS](https://www.earthcube.org/group/chords) project for real-time data services and extends the primary data models including site,instrument and variable, with additional metadata including adding spatial indexing and permissions. <br/>
The Streams API also integrates Tapis **event-driven** function such as [Abaco](https://tacc-cloud.readthedocs.io/projects/abaco/en/latest/) and **data management** and **code execution** capabilities to provide an analysis capability on streaming data sources.<br/>
 Support for streaming data includes the following capabilities:
 * Storing and retrieving streaming data for batch job processing, with support for temporal and spatial indexes and queries <br/>
 * Automated, event-driven data stream processing workflows with integration into Tapis functions as well as other streamingframeworks. <br/>

 *Real-time, event-driven workflows are supported by the Streams API. Tapis provides this capability through integration with its functions-as-a-service (Abaco), jobs service and other systems or services that support web-hooks. The Streams API provides the following capabilities to support various levels of analysis based on computational needs: <br/> 

 * Alerts as Events: Third-party processing engines will receive real-time notifications when measurement data hits pre-defined criteria. Subscribers will receive an HTTP POST request containing JSON data detailing the event that triggered the alert. <br/>
 * Processing Events with Tapis Functions— Developers are be able to register an Abaco function with an alert to performscalable processing with no infrastructure to maintain.<br/>


[Streams API Introduction Slides](https://docs.google.com/presentation/d/1NrTMVIMPqJIdungJ_kMF2FeXdVSwzDNWVhcJqyZhF_c/edit?usp=sharing)


