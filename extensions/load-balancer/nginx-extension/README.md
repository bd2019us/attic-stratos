# Apache Stratos Nginx Extension

Apache Stratos Nginx extension is a load balancer extension for Nginx. It is an executable program
which can manage the life-cycle of a Nginx instance according to the topology, composite application model,
tenant signups and domain mapping information received from Stratos via the message broker.

## How it works
1. Wait for the complete topology event message to initialize the topology.
2. Configure and start an instance of Nginx.
3. Listen to topology update messages.
4. Reload Nginx instance with the new topology configuration.