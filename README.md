# Note
- Solax X1-G4 Inverter (may not work with other inverters as settings and modes may be in different read/set positions)
- For reading live data you'll need my other [repo](https://github.com/RGx01/Solax-Local-Control-Using-REST) or [dashboard repo](https://github.com/RGx01/home-assistant-Solax-Zappi-Octopus-Control) 




# Install Instructions
1. In your Home Assistant /config directory create a directory (if one doesn't exist)
   * packages
2. Copy repo package directory to your package directory
3. Edit secrets.yaml to replace YYYYYYYYYY with your registration number (found on the devices page on the solax cloud)
4. Edit your configuration.yaml file (stored in the /config directory) to include:
```yaml
homeassistant:
  packages: !include_dir_merge_named packages/
```
5. Restart HA
