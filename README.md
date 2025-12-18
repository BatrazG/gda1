# gda1
# GoDedup

Утилита для поиска дубликатов файлов.

## Запуск

1. Сборка: `go build -o godedup ./cmd/dedup`
2. Запуск:

# Поиск по имени и размеру (быстро)
./godedup -path="./test_folder" -mode=name_size

# Поиск по хэшу (надежно, конкурентно)
./godedup -path="./test_folder" -mode=hash -workers=8

# Полный поиск (имя+размер, затем хэш)
./godedup -path="./test_folder" -mode=combined
