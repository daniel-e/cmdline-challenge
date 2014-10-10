'''
echo "abcdaefgh" | for i in `perl -pe 's#(.)#$1 #g'`; do echo $i; done | tac | tr -d "\n"; echo

echo "abcdaefgh" | grep . -o | cat -n | sort -rn | gawk '{print $2}' | tr -d \\n; echo

echo "abcdaefgh" | grep . -o | tac | tr -d \\n; echo
'''
