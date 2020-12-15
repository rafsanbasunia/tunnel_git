# tunnel_git

Fork the repo and run git actions. Use SSH_KEY in secrets to secure the tunnel.


By default it's only running qbittorrent in localhost:6565 , you can change the port on config.yml file.
To use qbittorent with ngrok follow these steps:
  1. Create a secret named NGROK_TOKEN and paste your ngrok authtoken.
  2. Start the workflow, wait for your tmate SSH link(usually take 4/5 minutes)
  3. Type this on terminal "ngrok http 6565". You'll be given a http and https link to access qbittorrent Web-ui.
