# TextProcessors
1. touch 1.txt
2. touch 2.txt
3. touch 3.txt
4. tail -n 40 1.txt | cat > 2.txt
5. head -n 10 2.txt | cat > 3.txt
6. sed -r 's/тах/трах/g' 2.txt | grep 'трах' | head -n 3 | cat >> 3.txt
7. sort 3.txt | uniq -c (при добовлении "| cat > 3.txt" файл очищается, но в него ничего не вставляется)
https://github.com/NikKokor/TextProcessors/raw/sort.jpg
