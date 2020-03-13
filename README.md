
Prometheus and statsd exporter metrics integration example
----------------------------------------------------------

## Run Docker Compose

    - docker-compose up

## Prometheus Listening Ports.

    View custom metrics in prometheus ui.

    - 0.0.0.0:9090

## Example for statsd

    echo "hits:ggjashd5757gjqw|c" | nc -u -w0 127.0.0.1 8125

    echo "failed:dkshj|c" | nc -u -w0 127.0.0.1 8125

## Example for statsd exporter

    echo "hits:ggjashd5757gjqw|c" | nc -u -w0 127.0.0.1 9125

    echo "failed:dkshj|c" | nc -u -w0 127.0.0.1 9125

--------------------------------------------------------------------------------

## Tips

`statsd` is not used in this setup since statsd exporter provides statsd server internally.

--------------------------------------------------------------------------------
