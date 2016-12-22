# xmodmapToshibaCB2
xmodmap (re)mappings for some keys, including: ñ ¿ Delete °
for the Toshiba Chromebook 2
I just put this in my .bashrc and voilá: Right Alt becomes Mode Switch, enabling some really useful mappings.
Might not be perfect. Sometimes i ahve to hit Ctrl+Alt+t because the mappings are spontaneously lost (though i almos never turn the chromebook off completely)

# F8
xmodmap -e "keycode  17 = 8 asterisk 8 F8 threequarters dead_ogonek threequarters"
# ¿
xmodmap -e "keycode  61 = slash question questiondown underscore questiondown dead_hook dead_belowdot abovedot"
# ñ
xmodmap -e "keycode 57 = n N ntilde Ntilde"
# Right alt as Mode Switch
xmodmap -e "keycode 108 = Mode_switch NoSymbol ISO_Level3_Shift"
# °
xmodmap -e "keycode  49 = dead_grave dead_tilde degree asciitilde grave asciitilde dead_grave dead_tilde"
# Delete
xmodmap -e "keycode  22 = BackSpace BackSpace Delete Delete BackSpace BackSpace"
