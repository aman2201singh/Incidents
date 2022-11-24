
| Incident ID | Symptoms                                                                                                        | Resolution                                                                                                                                                                                                                                                                                   | Reason                                                             |
|-------------|-----------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------|
| #134504     | (overall-rate-low  pulsar/astraproduction-azure-puls-prometheus critical)                                       | Message rate monitoring                                                                                                                                                                                                                                                                      |                                                                    |
| #132901     | Log query query result is > 1.0 for  2 minutes on 'Pulsar component  OutOfDirectMemoryError alert' By New Relic | we looked up the logs in new-relic  and found out that, this seems to  be the  broker issue.  We rolling  restarted the broker and also the  auto-recovery pod as it was  mentioned in the previous error  of the same kind, and we don't  see the out of memory errors in the logs anymore. | Due to heavy message transfer  that directly effects Direct Memory |
| #132536     | [FIRING:1]  (missing-function-critical  pulsar/astraproduction-aws-useast-prometheus critical)                  | A bad node was deleted for this.  pulsar-aws-useast1-function-0  belonging to this node was terminating  again and again. Cordoned the bad node, deleted pod to restart it to another node and deleted the node with issue.                                                                  | Pulsar-function pod not working  correctly                         |
| #132246     | pulsar-gcp-europewest1-broker-partition-topics-test:partition  topic test has over budget latency               | Broker restart                                                                                                                                                                                                                                                                               | Latency high for pub-sub latency  test at pulsar monitor           |
| #134808     | Broker StuckAstraCDCLogPartitionOrTopic pulsar                                                                  | Escalate for now  pulsar-admin topics unload  <topic name>                                                                                                                                                                                                                                   |                                                                    |
| #131609     | KubePersistentVolumeFillingUp                                                                                   | Changed pvc storage for from  50Gi to 100Gi                                                                                                                                                                                                                                                  | Journal/ledgers filling up                                         |
| #131251     | incluster-websocket-topic:websocket persisted latency  test failure                                             | DNS Restart/proxy restart                                                                                                                                                                                                                                                                    |                                                                    |
|             |                                                                                                                 |                                                                                                                                                                                                                                                                                              |                                                                    |


