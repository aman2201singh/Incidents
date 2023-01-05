## Persisted fenced topic on broker

**Description**  
The alert indicates that there is  fenced topic on broker.

**Diagnosis**  
Use this Splunk log query to search for the topics in fenced state https://datastax.splunkcloud.com/en-US/app/search/search?sid=1672851744.409174

**Mitigation**  
Identify all the topics in fenced state. If these topics are still in fenced state over 5 seconds, please manually unload them by pulsar-admin topics unload or from pulsar-admin-console UI
    

**Example**
