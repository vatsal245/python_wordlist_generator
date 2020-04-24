import itertools
import time
import sys

word_list = []
word_input = input("[+]Enter combination of words :>>")

length_minimum = int(input("[+]Enter minimum length :>>"))

length_maximum = int(input("[+]Enter maximum length :>>"))

wordlist_file = input("[+]Enter .txt file name :>>")

a = length_maximum + 1
k = 1

length_chrs = len(word_input)

for x in range(k, a):
    answer = length_chrs ** x
    word_list.append(answer)

line_sum = sum(word_list)
print("[+]No.of total combinations :>>",line_sum)

input("[+]Press enter once ready")

current_time = time.asctime()
start_time = time.time()

file_open = open(wordlist_file, 'a')

for n in range(k, a):
    g = n*100/a
    k = str(g) + 'percent'
    sys.stdout.write("\r%s" %k)
    sys.stdout.flush()
    file_open.flush()
    for x in itertools.product(word_input, repeat = n):
        file_open.write(''.join(x)+'\n')

file_open.flush()
file_open.close()

print("[+]wordlist generated successfully")
input("[+] Press any key to exit")

quit()
