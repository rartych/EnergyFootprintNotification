

| Item | Description | Support Qualifier |
|----|----|----|
|Summary|A Service Provider has requested the Telco Operator to instantiate applications in different Edge Data Centers. These applications, altogether, provide a Service offered to End Users via a mobile network. The Service Provider wants to know the E2E energy consumption and CO2 emission of its Service in a certain period of time. A system of the Service Provider invokes the Energy Footprint Notification API to get the above-mentioned information. The reported energy consumption and CO2 emissions consider the energy used to run the instances of the applications in the Data Centers and the energy consumption along the network to provide the Service (e.g., RAN and Core Network consumption) in the specified period of time.| M |
|Roles, Actor(s) and scope|Service Provider: role of EFN API consumer<br>API Provider: role of EFN API provider<br>Operator Platform ([EdgeCloud/documentation/SupportingDocuments/Edge terminology/edge_terminology.md at main · camaraproject/EdgeCloud](https://github.com/camaraproject/EdgeCloud/blob/main/documentation/SupportingDocuments/Edge%20terminology/edge_terminology.md)): role of Service host<br>Scope: Computing Services (OGW Taxonomy)| M |
|NF Requirements|NA| O |
|Pre-conditions|• The Service Provider onboarded applications on the Operator Platform<br>• The Service Provider requested the deployment of some instances of those applications<br>• The Service Provider identifies the Services as collection of application instances <br>• The Service provided by those instances is up and running.| M |
|Begins when|The API Consumer invokes the EFN API to get the Energy consumption of the Service, composed by a set of application instances, in a specific time period.| M |
|Step 2|The API Provider returns the overall Energy consumption of the Service in that specific time period.| M|
|Step 4|The API Consumer invokes the EFN API to get the Carbon footprint of the Service, composed by a set of application instances, in a specific time period.| M |
|Step 5|The API Provider returns the Carbon footprint of the Service in that specific time period.| M|
|Post-conditions|The Service Provider is aware of the Energy consumption and of the Carbon footprint of the Service in the selected time periods| M |
