## ttn broker

The Things Network broker

### Synopsis


ttn broker starts the Broker component of The Things Network.

The Broker is responsible for finding the right handler for uplink packets it
receives from Routers. Handlers have register Applications and personalized
devices (with their network session keys) with the Broker.
	

```
ttn broker
```

### Options

```
      --applications_database string   Applications Database connection (default "boltdb:/tmp/ttn_apps_broker.db")
      --devices_database string        Devices Database connection (default "boltdb:/tmp/ttn_devs_broker.db")
      --downlink-address string        The IP address to listen for downlink communication (default "0.0.0.0")
      --downlink-port int              The port for downlink communication (default 1781)
      --status-address string          The IP address to listen for serving status information (default "0.0.0.0")
      --status-port int                The port of the status server, use 0 to disable (default 10701)
      --uplink-address string          The IP address to listen for uplink communication (default "0.0.0.0")
      --uplink-port int                The port for uplink communication (default 1881)
```

### Options inherited from parent commands

```
      --config string   config file (default "$HOME/.ttn.yaml")
```

### SEE ALSO
* [ttn](ttn)	 - The Things Network's backend servers

###### Auto generated by spf13/cobra on 23-Mar-2016