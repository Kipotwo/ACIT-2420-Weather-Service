# ACIT-2420-Weather-Service

Using this weather service is easy!

Step 1:
Move wttr into any directory you please, as long as you remember the path.

Step 2:
Move wttr.service and wttr.timer into /etc/systemd/system

Step 3:
Configure wttr.service to have
    - ExecStart be the path to wttr file
    - WorkingDirectory be the path to the directory wttr file is in.

Step 4:
Run sudo systemctl daemon-reload

Step 5:
Run "sudo systemctl enable --now wttr.timer" to enable the timer

Step 6:
Start wttr.service and wttr.timer using "sudo systemctl start wttr.service" 
and "sudo systemctl start wttr.timer"

Congratulations!
You have set up the wttr service!
