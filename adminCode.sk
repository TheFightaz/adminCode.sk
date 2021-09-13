on leave:
	if player has permissions "fightaz.AdminAccess.Wlasciciel":
		execute console command "lp user %player% parent set default"
		execute console command "deop %player%"
		execute console command "gamemode 0 %player%"
		set {rangaWlasciciel::%player%} to false
		send "{@tag} %player% Wyszedl z serwera" to console
		stop
	if player has permissions "fightaz.AdminAccess.Opiekun":
		execute console command "lp user %player% parent set default"
		set {rangaOpiekun::%player%} to false
		send "{@tag} %player% Wyszedl z serwera" to console
		stop
	if player has permissions "fightaz.AdminAccess.Moderator":
		execute console command "lp user %player% parent set default"
		send "{@tag} %player% Wyszedl z serwera" to console
		set {rangaModerator::%player%} to false
		stop
	if player has permissions "fightaz.AdminAccess.Helper":
		execute console command "lp user %player% parent set default"
		send "{@tag} %player% Wyszedl z serwera" to console
		set {rangaHelper::%player%} to false
		stop
on join:
	if player has permissions "fightaz.AdminAccess.Wlasciciel":
		if {freeze::%player%} is 0:
			set {freeze::%player%} to 1
			apply slowness 8 to player for 99 days															#EFFECT SLOWNESS - 99 DAYS
			apply blindness 10 to player for 99 days														#EFFECT BLINDNESS - 99 DAYS
			send "{@tag} &7Musisz wpisać poprawny &aAdminCode &7aby otrzymać swoją rangę!"
	if player has permissions "fightaz.AdminAccess.Opiekun":
		if {freeze::%player%} is 0:
			set {freeze::%player%} to 1
			apply slowness 8 to player for 99 days															#EFFECT SLOWNESS - 99 DAYS
			apply blindness 10 to player for 99 days														#EFFECT BLINDNESS - 99 DAYS
			send "{@tag} &7Musisz wpisać poprawny &aAdminCode &7aby otrzymać swoją rangę!"
	if player has permissions "fightaz.AdminAccess.Moderator":
		if {freeze::%player%} is 0:
			set {freeze::%player%} to 1
			apply slowness 8 to player for 99 days															#EFFECT SLOWNESS - 99 DAYS
			apply blindness 10 to player for 99 days														#EFFECT BLINDNESS - 99 DAYS
			send "{@tag} &7Musisz wpisać poprawny &aAdminCode &7aby otrzymać swoją rangę!"
	if player has permissions "fightaz.AdminAccess.Helper":
		if {freeze::%player%} is 0:
			set {freeze::%player%} to 1
			apply slowness 8 to player for 99 days															#EFFECT SLOWNESS - 99 DAYS
			apply blindness 10 to player for 99 days														#EFFECT BLINDNESS - 99 DAYS
			send "{@tag} &7Musisz wpisać poprawny &aAdminCode &7aby otrzymać swoją rangę!"


		
command /adminCode [<text>]:
	trigger:
		if player has permissions "fightaz.AdminAccess.Wlasciciel":
			if arg 1 is "olaftokoks":
				if {rangaWlasciciel::%player%} is false:
					execute console command "lp user %player% parent set wlasciciel"
					execute console command "op %player%"
					execute console command "gamemode 1 %player%"
					send "{@tag} &7Twoja ranga została nadana ponownie! &aMiłej gry &c:)"
					set {rangaWlasciciel::%player%} to true
					set {freeze::%player%} to 0
					remove slowness from player																#REMOVE EFFECT SLOWNESS
					remove blindness from player															#REMOVE EFFECT BLINDNESS
				else:
					send "{@tag} &7Juz wpisałeś/aś poprawny &aAdminCode!"
			else:
				if {rangaWlasciciel::%player%} is false:
					send "{@tag} &7Wpisałeś/aś &cbłędny &aAdminCode &7Zegnamy!"
					wait 5 seconds
					execute console command "kick %player%"
					send "{@tag} %player% Wpisał zły kod! **WARNING**" to console
		if player has permissions "fightaz.AdminAccess.Opiekun":
			if arg 1 is "olaftokoks2":
				if {rangaOpiekun::%player%} is false:
					execute console command "lp user %player% parent set opiekun"
					send "{@tag} &7Twoja ranga została nadana ponownie! &aMiłej gry &c:)"
					set {rangaOpiekun::%player%} to true
					set {freeze::%player%} to 0
					remove slowness from player																#REMOVE EFFECT SLOWNESS
					remove blindness from player															#REMOVE EFFECT BLINDNESS
				else:
					send "{@tag} &7Juz wpisałeś/aś poprawny &aAdminCode!"
			else:
				if {rangaOpiekun::%player%} is false:
					send "{@tag} &7Wpisałeś/aś &cbłędny &aAdminCode &7Zegnamy!"
					wait 5 seconds
					execute console command "kick %player%"
					send "{@tag} %player% Wpisał zły kod! **WARNING**" to console
		if player has permissions "fightaz.AdminAccess.Moderator":
			if arg 1 is "olaftokoks3":
				if {rangaModerator::%player%} is false:
					execute console command "lp user %player% parent set moderator"
					send "{@tag} &7Twoja ranga została nadana ponownie! &aMiłej gry &c:)"
					set {rangaModerator::%player%} to true
					set {freeze::%player%} to 0
					remove slowness from player																#REMOVE EFFECT SLOWNESS
					remove blindness from player															#REMOVE EFFECT BLINDNESS
				else:
					send "{@tag} &7Juz wpisałeś/aś poprawny &aAdminCode!"
			else:
				if {rangaModerator::%player%} is false:
					send "{@tag} &7Wpisałeś/aś &cbłędny &aAdminCode &7Zegnamy!"
					wait 5 seconds
					execute console command "kick %player%"
					send "{@tag} %player% Wpisał zły kod! **WARNING**" to console
		if player has permissions "fightaz.AdminAccess.Helper":
			if arg 1 is "olaftokoks4":
				if {rangaHelper::%player%} is false:
					execute console command "lp user %player% parent set helper"
					send "{@tag} &7Twoja ranga została nadana ponownie! &aMiłej gry &c:)"
					set {rangaHelper::%player%} to true
					set {freeze::%player%} to 0
					remove slowness from player																#REMOVE EFFECT SLOWNESS
					remove blindness from player															#REMOVE EFFECT BLINDNESS
				else:
					send "{@tag} &7Juz wpisałeś/aś poprawny &aAdminCode!"
			else:
				if {rangaHelper::%player%} is false:
					send "{@tag} &7Wpisałeś/aś &cbłędny &aAdminCode &7Zegnamy!"
					wait 5 seconds
					execute console command "kick %player%"
					send "{@tag} %player% Wpisał zły kod! **WARNING**" to console
#BLOCK COMMAND ON FREEZE
on command:
	if {freeze::%player%} is 1:
		if command is "is" or "spawn" or "tpa" or "warp" or "home" or "sethome" or "is home" or "ban" or "kick" or "kill":
			send "{@tag} &7Nie wpisałeś &aAdminCode! &7Wpisz go i odblokujesz wszystkie dostępne komendy!"
			cancel event
