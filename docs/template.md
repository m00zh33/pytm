# Threat Model Sample
***

## System Description

{tm.description}

## Dataflow Diagram

![Level 0 DFD](dfd.png)


## Dataflows

Name|From|To |Data|Protocol|Port
----|----|---|----|--------|----
{dataflows:repeat:{{item.name}}|{{item.source.name}}|{{item.sink.name}}|{{item.data}}|{{item.protocol}}|{{item.dstPort}}
}


## Potential Threats

{findings:repeat:* {{item.description}} on element "{{item.target}}"
}
