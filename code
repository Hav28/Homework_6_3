import os
number_1text = {}
for file in os.listdir('files'):
    with open(os.path.join('files', file), encoding='utf-8') as f:
        text = f.readlines()
        text_ = "".join(text)
        len_ = len(text)
        number_1text[file] = (f'{len_}\n{text_}\n')
        print(number_1text[file])
number_2text = {}
for x in sorted(number_1text, key=number_1text.get):
    # print(x)
    number_2text[x] = number_1text[x]
    # print(number_2text[x])
for key, value in number_2text.items():
    with open('full_files.txt', 'a', encoding='utf-8') as f:
        f.writelines(f'{key}\n{value}\n')
