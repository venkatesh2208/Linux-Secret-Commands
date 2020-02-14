# LINUX SECRET COMMANDS 

# BELOW ARE THE SOME OF THE SIMPLE AND ADVANCED COMMAND THAT YOU CAN TRY ON YOU LINUX SYSTEM





# GET WIFI PASSWORD
  >" cat /etc/NetworkManager/system-connections/[SSID] | grep psk= "
  
# LIST NETWORK INTERFACES
  >lspci | egrep -i --color 'network|ethernet'
  
# GET YOUR FIREFOX HISTORY 
  >sqlite3 ~/.mozilla/firefox/*.[dD]efault/places.sqlite "SELECT strftime('%d.%m.%Y %H:%M:%5',visit_date/1000000, 'unixepoch'.'localtime'),url FROM moz_places,moz_historyvisits WHERE moz_places.id=moz_historyvisits.places_id ORDER BY visit_date;"

# CHECK ALL BASH SCRIPTS IN CURRENT DIR FOR SYSTAX ERRORS
  >find . -name '*sh' -exer bash -n {} \;
 
# LIST DIRECTORIES ONLY
  >ls -d */

# WATCH YOUR NETWORK SERVICE ACTIVITY IN REAL-TIME
  >lsof -i
  
# ESCAPE ANY COMMAND ALIASES
  >/[command]

# KILLS A PROCESS THAT IS LOCKING A FILE
  > fuser -k [filename]
