# Log Forwarder Configuration. 

Checkout the [log forwarder-recevier documentation](https://doc.punchplatform.com/Operations/Reference_Architecture/Log_Collector.html). The channel illustrated here is a simpler variant that provides four punchlines: 

* ltr_in : tcp input (port 9902) to kafka topic 'ltr'
* ltr_out: kafka to lumberjack lmr_in (port 2001)
* lmr_in lumberjack (port 2001) to kafka topic 'lmr'
* lmr_out : Kafka topic 'lmr' to stdout


Start you channel

```sh
channelctl --tenant samples --channel lrt_lmr
```

Then inject some traffic: 

```sh
punchplatform-log-injector -c injector.json
```

