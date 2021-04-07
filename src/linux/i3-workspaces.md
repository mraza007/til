# Assigning Programs to Workspaces

To open programs on specific windows when using `i3` window mananger add the  following to the i3 config

`assign [class="<use your program name here e.g. - Firefox>"] $workspace <eg 5>`

After adding to the config make sure to refresh `i3-msg reload`