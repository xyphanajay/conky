-- vim: ts=4 sw=4 noet ai cindent syntax=lua


conky.config = {
    alignment = 'top_left',
    background = false,
    border_width = 0.5,
    cpu_avg_samples = 4,
    default_color = 'white',
    default_outline_color = 'grey',
    default_shade_color = 'black',
    draw_borders = true,
    draw_graph_borders = true,
    draw_outline = false,
    draw_shades = false,
    use_xft = true,
    font = 'DejaVu Sans Mono:size=10',
    gap_x = 5,
    gap_y = 50,
    minimum_height = 5,
    minimum_width = 5,
    net_avg_samples = 2,
    double_buffer = true,
    out_to_console = false,
    out_to_stderr = false,
    extra_newline = false,
    own_window = true,
    own_window_colour = '000000',
    own_window_class = 'Conky',
    own_window_argb_visual = true,
    own_window_argb_count = 0,
    own_window_type = 'dock',
    own_window_transparent = true,
    own_window_hints = 'undecorated,below,sticky,skip_taskbar,skip_pager',
    stippled_borders = 0,
    update_interval = 1,
    uppercase = false,
    use_spacer = 'none',
    show_graph_scale = false,
    show_graph_range = false
}

conky.text = [[
${font DejaVu Sans Mono:size=14}${alignc}${time %I:%M:%S}
${font Impact:size=10}${alignc}${time %A, %B %e, %Y}
${font Entopia:size=12}${color orange}CALENDAR ${hr 2}$color
${font DejaVu Sans Mono:size=9}${execpi 1800 DA=`date +%_d`; cal | sed s/"\(^\|[^0-9]\)$DA"'\b'/'\1${color orange}'"$DA"'$color'/}
${font Entopia:bold:size=12}${color red}FILE SYSTEM ${hr 2}${font Noto sans:size=8}
#${offset 4}${color}dev ${alignr}FREE     USED
${offset 4}${color}root (${fs_type /}) ${color yellow}${alignr}${fs_free /} ${fs_used /}
${offset 4}${color yellow}${fs_size /} ${color}${fs_bar 4 /}
${offset 4}${color FFFDE2}home (${fs_type /home}) ${color yellow}${alignr}${fs_free /home/} ${fs_used /home/}
${offset 4}${color yellow}${fs_size /home/} $color${fs_bar 4 /home/}
${offset 4}${color FFFDE2}sda5 (${fs_type /run/media/senpai/6EC832DEC832A3ED/}) ${color yellow}${alignr}${fs_free /run/media/senpai/6EC832DEC832A3ED/} ${fs_used /run/media/senpai/6EC832DEC832A3ED/}
${offset 4}${color yellow}${fs_size /run/media/senpai/6EC832DEC832A3ED/} $color${fs_bar 4 /run/media/senpai/6EC832DEC832A3ED/}
${offset 4}${color FFFDE2}sda6 (${fs_type /run/media/senpai/6EC832DEC832A3ED/}) ${color yellow}${alignr}${fs_free /run/media/senpai/C208F88708F87BAB/} ${fs_used /run/media/senpai/C208F88708F87BAB/}
${offset 4}${color yellow}${fs_size /run/media/senpai/C208F88708F87BAB/} $color${fs_bar 4 /run/media/senpai/C208F88708F87BAB/}
${font Entopia:bold:size=12}${color green}CPU ${hr 2}
${offset 4}${color black}${cpugraph F600AA 5000a0}
${offset 4}${font DejaVu Sans Mono:size=9}${color white}CPU: $cpu% ${color red}${cpubar 6}
${font Entopia:bold:size=12}${color 00FFD0}Network ${hr 2}  
${color black}${downspeedgraph enp8s0 32,80 ff0000 0000ff}${color black}${upspeedgraph enp8s0 32,80 0000ff ff0000}
$color${font DejaVu Sans Mono:size=8}▼ ${downspeed enp8s0}${alignc}${color green} IPv6${alignr}${color}▲ ${upspeed enp8s0}
${color black}${downspeedgraph wlp10s0f0 32,80 ff0000 0000ff}${color black}${upspeedgraph wlp10s0f0 32,80 0000ff ff0000}
$color${font DejaVu Sans Mono:size=8} ▼ ${downspeed wlp10s0f0}${alignc}${color orange} ${wireless_essid wlp10s0f0}${alignr}${color}▲ ${upspeed wlp10s0f0}
${font Entopia:bold:size=12}${color F600AA}Disk I/O ${hr 2}
${alignc}${font}${color white}SSD vs HDD $mpd_name
${color black}${diskiograph /dev/sda 32,80 a0af00 00110f}${diskiograph /dev/sdb 32,80 f0000f 0f0f00}
${font DejaVu Sans Mono:size=8}${color white}   ${diskio /dev/sda}${alignr}${diskio /dev/sdb}
]]
