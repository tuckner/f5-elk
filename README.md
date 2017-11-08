# f5-elk
### Logstash Configs and Kibana Dashboards for F5 LTM &amp; ASM

Logstash input, filter, output, and mapping template used to store F5 LTM and ASM logs.  Presented at the Kansas City F5 User Group.

https://johntuckner.me/2017/02/20/elk-integrating-f5-ltm-and-asm/

##### Logstash Directory Structure:

```
/etc/logstash
├── /conf.d                    # Logstash conf directory
│   ├── 01-f5-input.conf          # Input configurations
│   ├── 20-f5-filter.conf         # Filter configurations
│   └── 40-f5-output.conf         # Output configurations
└─ /templates                  # Logstash templates for Elasticsearch
│   └── f5-template.json          # Template used for F5 mappings
```

##### Kibana Dashboards and Visualizations:

Import the kibana-export.json file into your Kibana instace:

`Management -> Saved Objects -> Dashboards -> Import`
