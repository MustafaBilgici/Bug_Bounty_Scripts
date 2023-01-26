

Extract all URL from Source Code✨

curl domain.com | grep -oP '(https*.//|www\.)[^]*'

## sed

Run replacements based on regular expressions.

- Replace the first occurrence of a string in a file, and print the result:

sed 's/find/replace/' filename

- Replace only on lines matching the line pattern:

sed '/line_pattern/s/find/replace/'

- Replace all occurrences of a string in a file, overwriting the file (i.e. in-place):

sed -i 's/find/replace/g' filename

- Replace all occurrences of an extended regular expression in a file:

sed -r 's/regex/replace/g' filename

- Apply multiple find-replace expressions to a file:

sed -e 's/find/replace/' -e 's/find/replace/' filename

$ tldr awk

## awk

A versatile programming language for working on files.

- Print the fifth column in a space separated file:

awk '{print $5}' filename

- Print the second column of the lines containing "something" in a space separated file:

awk '/something/ {print $2}' filename

- Print the third column in a comma separated file:

awk -F ',' '{print $3}' filename

- Sum the values in the first column and print the total:

awk '{s+=$1} END {print s}' filename

- Sum the values in the first column and pretty-print the values and then the total:

awk '{s+=$1; print $1} END {print "--------"; print s}' filename

𝙓𝙎𝙎 𝙊𝙣𝙚𝙡𝙞𝙣𝙚𝙧 𝙆𝙖𝙩𝙖𝙣𝙖 ✚ 𝘿𝙖𝙡𝙛𝙤𝙭

echo domain.com | katana -jc -f qurl -d 5 -c 50 -kf robotstxt,sitemapxml -silent | dalfox pipe --skip-bav