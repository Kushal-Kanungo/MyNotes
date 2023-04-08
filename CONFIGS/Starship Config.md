Copy this file in `~/.config/starship.toml`
```toml
format = """
$username\
$kubernetes\
$directory\
$git_branch\
$git_commit\
$git_state\
$git_status\
$hg_branch\
$docker_context\
$package\
$cmake\
$dart\
$deno\
$dotnet\
$elixir\
$elm\
$erlang\
$golang\
$helm\
$java\
$julia\
$kotlin\
$nim\
$ocaml\
$perl\
$php\
$purescript\
$python\
$red\
$rust\
$swift\
$terraform\
$vlang\
$vagrant\
$zig\
$nix_shell\
$conda\
$aws\
$gcloud\
$openstack\
$env_var\
$crystal\
$custom\
$cmd_duration\
$lua\
$fill\
$nodejs\
$ruby\
$line_break\
$jobs\
$character"""

scan_timeout = 10

add_newline = false

[battery]
disabled = false

[character]
success_symbol = "[](blue)"
error_symbol = "[](bright-red)"

[cmd_duration]
show_notifications = true
min_time_to_notify = 60_000

[directory]
truncation_length = 1
format = "[](blue) [$path]($style)[$read_only]($read_only_style)"
read_only = " "
truncation_symbol = ""
fish_style_pwd_dir_length = 0

[git_branch]
format = ":[$symbol$branch]($style)"
symbol = " "
truncation_length = 16

[git_state]
format = '\(:[$state( $progress_current/$progress_total)]($style)\)'

[git_status]
format = '(:[$all_status$ahead_behind]($style)) '
conflicted = '\[ [$count](bright-white bold)\]'
ahead = '\[[ ](bright-blue)[$count](bright-white bold)\]'
behind = '\[[ ](white)[$count](bright-white bold)\]'
diverged = '\[[ ](purple)|[ ﯁ ](bright-blue)[$ahead_count](bright-white bold)[ ﮾ ](white)[$behind_count](bright-white)\]'
untracked = '\[U:[$count](bright-white bold)\]'
stashed = '\[[S:](bright-green)[$count](bright-white bold)\]'
modified = '\[[M:](bright-yellow)[$count](bright-white bold)\]'
staged = '\[[ ](bright-green)[$count](bright-white bold)\]'
renamed = '\[[ ](bright-cyan) [$count](bright-white bold)\]'
deleted = '\[[ [$count](bright-white bold)\]'

[python]
format = 'via [${symbol}${pyenv_prefix}(${version} )(\($virtualenv\) )]($style)'

[ruby]
symbol = '󰴭 '
format = '[$symbol($version )]($style)'

[fill]
symbol = ' '

[nodejs]
format = '[$symbol($version )]($style)'

[hostname]
disabled = true
```