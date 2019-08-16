# nukijuan

Workaround in order to use nuki lock in HA > 0.97.x avoiding the unavailable state.

This component is based in the HA one but will retry the connection in order to avoid 503 errors and the unresponsible nuki API.

Copy all files to /custom_components/nukijuan and in your configuration.yaml add the following:

lock:
  - platform: nukijuan
    host: 192.168.1.42
    port: 8080
    token: xxxx


