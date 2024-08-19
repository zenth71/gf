- name: Debug Ngrok
  run: |
    ngrok tcp 3389 -log=stdout > ngrok_log.txt &
    sleep 10
    cat ngrok_log.txt
