# MyFerstRepro
Мой первый репозиторий
things = {'карандаш': 20, 'зеркальце': 100, 'зонт': 500, 'рубашка': 300,
          'брюки': 1000, 'бумага': 200, 'молоток': 600, 'пила': 400, 'удочка': 1200,
          'расческа': 40, 'котелок': 820, 'палатка': 5240, 'брезент': 2130, 'спички': 10}
n = int(input())*1000
spis_key = []
for key, val in sorted(things.items(),key=lambda x: -x[1]):
    if n >= val:
        spis_key.append(key)
        n -= val
print(*spis_key)
