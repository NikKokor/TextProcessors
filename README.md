# TextProcessors
1. touch 1.txt
2. touch 2.txt
3. touch 3.txt

![Image alt](https://github.com/NikKokor/TextProcessors/raw/main/image1.jpg)

4. tail -n 40 1.txt | cat > 2.txt

![Image alt](https://github.com/NikKokor/TextProcessors/raw/main/image2.jpg)

5. head -n 10 2.txt | cat > 3.txt

![Image alt](https://github.com/NikKokor/TextProcessors/raw/main/image3.jpg)

6. sed -r 's/тах/трах/g' 2.txt | grep 'трах' | head -n 3 | cat >> 3.txt

![Image alt](https://github.com/NikKokor/TextProcessors/raw/main/image4.jpg)

7. sort 3.txt | uniq -c (при добовлении "| cat > 3.txt" файл очищается, но в него ничего не вставляется)

![Image alt](https://github.com/NikKokor/TextProcessors/raw/main/sort.jpg)
