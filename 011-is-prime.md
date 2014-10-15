echo "17" | seq `cat` -1 2 | cat -n | gawk '{print $1+$2-1}' | cat -n | tail -n +2 | gawk '{print $2%$1}' | grep '^0$' | wc -l
