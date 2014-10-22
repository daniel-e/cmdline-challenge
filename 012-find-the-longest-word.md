echo -e "ab\nabc\naduib\niu\nuzdf\n12345" | awk '{print length, $0}' | sort -nr | head -1 | cut -d\  -f2

sed 's#.*#echo `echo & | wc -c` &#e'
